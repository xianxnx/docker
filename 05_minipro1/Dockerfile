FROM quay.io/centos/centos:stream10

RUN dnf -y install vsftpd && yum clean all

COPY vsftpd.conf.template /etc/vsftpd/vsftpd.conf

COPY WelcomeToMyFTPServer.txt /var/ftp/pub/

VOLUME /var/ftp/pub

EXPOSE 21/tcp
EXPOSE 20/tcp

ENTRYPOINT ["/usr/sbin/vsftpd"]
