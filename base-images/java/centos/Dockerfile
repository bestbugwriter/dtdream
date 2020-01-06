FROM centos:centos7.2.1511

ENV LANG en_US.UTF-8

# Set timezone
ENV TZ=Asia/Shanghai
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

# install openjdk8
RUN yum install --assumeyes --quiet java-1.8.0-openjdk-devel net-tools iproute2 wget less && yum clean all

# Set JAVA_TOOL_OPTIONS
ENV JAVA_TOOL_OPTIONS="-Dfile.encoding=UTF-8 -Dsun.jnu.encoding=UTF-8"

# Set JAVA_HOME
ENV JAVA_HOME=/usr/lib/jvm/java
