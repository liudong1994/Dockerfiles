FROM centos:7.3.1611

LABEL cpp-builder-version="1.1"
LABEL cpp-builder-date="2020-07-15 10:00"

RUN echo "/usr/local/lib64/" >> /etc/ld.so.conf \
  && ldconfig \
  && ulimit -c unlimited \
  && rm -f /etc/localtime \
  && ln -sv /usr/share/zoneinfo/Asia/Shanghai /etc/localtime \
  && echo "Asia/Shanghai" > /etc/timezone

RUN yum install -y gcc-c++ \
  && yum install -y cmake \
  && yum install -y mysql-devel \
  && yum install -y boost-devel \
  && yum install -y libtool \
  && yum install -y libuuid-devel \
  && yum install -y rpm-build \
  && yum install -y rsync \
  && yum install -y curl-devel \
  && yum install -y wget \
  && yum install -y cmake \
  && yum install -y vim \
  && yum install -y lrzsz

