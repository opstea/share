`docker-compose.yml`是 zabbix server 端一键起服务配置。
提前安装好`docker docker-compose`

```shell
# 创建目录。下载docker-compose.yml 文件，下载中文字体包。
mkdir -pv /data/zabbix/{alertscript,db,fonts}
cd /data/zabbix
wget https://raw.githubusercontent.com/opstea/share/master/zabbix/docker-compose.yml
wget https://raw.githubusercontent.com/opstea/share/master/zabbix/msyh.ttc -O /data/zabbix/fonts/DejaVuSans.ttf

docker-compose up -d 

```