FROM centos:7
MAINTAINER blankhang <blankhang@gmail.com>
LABEL version='1.0' description='centos7 with chinese lanugage and openjdk11 and CST GMT+8 timezone support'

RUN yum install -y libXmu freetype kde-l10n-Chinese fontconfig && yum -y reinstall glibc-common && yum groupinstall "fonts" -y && fc-cache -fv && localedef -c -f UTF-8 -i zh_CN zh_CN.utf8 && cp /usr/share/zoneinfo/Asia/Shanghai /etc/localtime && echo "Asia/Shanghai" > /etc/timezone && yum install -y java-11-openjdk && yum clean all && rm -rf /var/cache/yum/*