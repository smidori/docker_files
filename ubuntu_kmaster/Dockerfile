FROM ubuntu:latest
MAINTAINER silvia shimabuko
RUN echo kmaster > /etc/hostname
RUN apt-get update
RUN apt-get install -y curl
RUN apt-get install -y gnupg
RUN apt-get install -y software-properties-common
RUN apt-get install -y net-tools
RUN curl -s https://packages.cloud.google.com/apt/doc/apt-key.gpg | apt-key add -
RUN apt-add-repository "deb http://apt.kubernetes.io/ kubernetes-xenial main"
#apt-get update
RUN apt-get install -y kubelet kubeadm kubectl
#kubectl version
RUN apt-get install openssh-server