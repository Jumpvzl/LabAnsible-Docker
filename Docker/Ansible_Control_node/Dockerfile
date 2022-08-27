FROM centos
ENV ANSIBLE_HOST_KEY_CHECKING False
RUN sed -i -e "s|#baseurl=http://mirror.centos.org|baseurl=http://vault.centos.org|g" /etc/yum.repos.d/CentOS-* && yum install epel-release -y && yum update -y && yum install -y openssh-server openssh-clients net-tools && yum install -y ansible
CMD /bin/bash
