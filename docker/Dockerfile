FROM scratch
MAINTAINER HQM <hakim@detik.com>
ADD c68-docker.tar.xz /
LABEL name="CentOS Base Image" \
    vendor="CentOS" \
    license="GPLv2" \
    build-date="2018-01-02"

ADD ffmpeg.tar.xz /bin 

ENTRYPOINT ["/bin/ffmpeg"]
