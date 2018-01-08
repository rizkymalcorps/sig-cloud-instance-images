FROM scratch
MAINTAINER HQM <hakim@detik.com>
ADD c68-docker.tar.xz /
LABEL name="CentOS Base Image" \
    vendor="CentOS" \
    license="GPLv2" \
    build-date="2018-01-02"

RUN apt-get update && apt-get install  libgtk2.0-0:i386 libidn11:i386 libglu1-mesa:i386

ADD ffmpeg.tar.xz /bin 

ENTRYPOINT ["/bin/ffprobe"]
