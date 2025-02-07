ARG baseimage=meldsun/samba
ARG tag=25.2-develop-a8a0424-2
FROM $baseimage:$tag
RUN echo "latest" > /version.txt

ENTRYPOINT ["samba-entry.sh"]


USER root

ADD samba.sh /opt/samba/bin/samba.sh
RUN chmod +x /opt/samba/bin/samba.sh
ENTRYPOINT ["/opt/samba/bin/samba.sh"]

