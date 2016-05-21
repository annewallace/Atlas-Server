FROM ubuntu:14.04
MAINTAINER Denis Carriere <Carriere.Denis@gmail.com>

ADD atlas-server-linux-x64-v0.8.1 /src
RUN ["/src/install.sh"]

EXPOSE 2999
CMD ["/opt/atlas-server/etc/start.sh"]
