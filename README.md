Please Follow Alibaba Office Help Doc:
https://github.com/alibaba/canal/wiki/Docker-QuickStart

Some change?
1. Change netmode from host to bridge
2. Add links in order to user local mysql server

How to setup canal server?

./run.sh -e canal.auto.scan=false \
                  -e canal.destinations=test \
                  -e canal.instance.master.address=db:3306\
                  -e canal.instance.dbUsername=canal\
                  -e canal.instance.dbPassword=canal.123\
                  -e canal.instance.connectionCharset=UTF-8 \
                  -e canal.instance.tsdb.enable=true \
                  -e canal.instance.gtidon=false  \

