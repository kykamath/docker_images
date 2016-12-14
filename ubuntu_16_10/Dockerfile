# docker build -t kykamath/ubuntu_16_10:base .
# docker run -it kykamath/ubuntu_16_10:base
# docker push kykamath/ubuntu_16_10:base
FROM ubuntu:16.10
MAINTAINER Krishna Y. Kamath <krishna.kamath@gmail.com>

# install basic libs
RUN apt-get update && \
  apt-get install -y build-essential checkinstall && \
  apt-get install -y libreadline-gplv2-dev libncursesw5-dev libssl-dev libsqlite3-dev tk-dev libgdbm-dev libc6-dev libbz2-dev wget

# install python
RUN  cd /usr/src && \
  wget https://www.python.org/ftp/python/2.7.12/Python-2.7.12.tgz && \
  tar xzf Python-2.7.12.tgz && \
  cd Python-2.7.12 && \
  ./configure && \
  make install
