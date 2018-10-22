# Version: 0.0.1
# edt M06 2018-2019
# ldapserver base edt.org
#-------------------------------------------------
FROM fedora:27
LABEL author="@edt ASIX M06-ASO"
LABEL description="ldaphost 2018-2018 ldapserver"
RUN dnf -y install procps openldap-clients openldap-servers
RUN mkdir /opt/docker
COPY * /opt/docker/
RUN chmod +x /opt/docker/install.sh /opt/docker/startup.sh
WORKDIR /opt/docker
CMD ["bin/bash"]

