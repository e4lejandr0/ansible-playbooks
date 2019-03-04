FROM centos:centos7

RUN yum upgrade -y

RUN yum install -y  https://downloads.plex.tv/plex-media-server/1.14.1.5488-cc260c476/plexmediaserver-1.14.1.5488-cc260c476.x86_64.rpm

USER plex

WORKDIR "/usr/lib/plexmediaserver"

ENV LD_LIBRARY_PATH=/usr/lib/plexmediaserver
ENV "PLEX_MEDIA_SERVER_APPLICATION_SUPPORT_DIR=/var/lib/plexmediaserver/Library/Application Support"
ENV "PLEX_MEDIA_HOME=/usr/lib/plexmediaserver"
ENV "PLEX_MEDIA_SERVER_MAX_PLUGIN_PROCS=6"
ENV "PLEX_MEDIA_SERVER_TMPDIR=/tmp"
ENV "LC_ALL=en_US.UTF-8"
ENV "LANG=en_US.UTF-8"
ENV "PLEX_CLAIM=claim-zDHU6b1oGZGVUJZnpuRa"

EXPOSE 32400/tcp


ENTRYPOINT [ "/usr/lib/plexmediaserver/Plex Media Server" ]

