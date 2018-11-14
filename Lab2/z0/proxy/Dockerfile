 FROM  sameersbn/squid:latest
 RUN apt-get update && \
    apt-get -y install apache2-utils iproute2 && \
    apt-get -y install wget && \
    htpasswd -bmc /etc/squid/passwd user password && \
    htpasswd -bm /etc/squid/passwd user1 password1 && \
    htpasswd -bm /etc/squid/passwd user2 password2 && \
    chmod o+r /etc/squid/passwd
EXPOSE 3128
