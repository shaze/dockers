

FROM docker.io/jenkins/jenkins:lts
USER root
RUN apt-get update && \
apt-get -y install build-essential checkinstall &&\
apt-get -y install libreadline-gplv2-dev libncursesw5-dev libssl-dev     libsqlite3-dev tk-dev libgdbm-dev libc6-dev\
                libbz2-dev libffi-dev && \
wget https://www.python.org/ftp/python/3.7.2/Python-3.7.2.tgz && \
tar xzf Python-3.7.2.tgz && \
cd Python-3.7.2  && \
./configure --enable-optimizations --with-ensurepip=install && \
make altinstall && \
pip3.7 install --upgrade pip && \ 
pip3.7 install matplotlib
USER jenkins
