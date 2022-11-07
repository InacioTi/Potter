FROM mariadb:latest

RUN echo "nameserver 8.8.8.8" > /etc/resolv.conf

RUN apt update 

ADD ./startup.sh /scripts/startup.sh
RUN chmod -R 755 /scripts

EXPOSE 3306

VOLUME ["/var/lib/mysql"]

ENTRYPOINT ["/scripts/startup.sh"]