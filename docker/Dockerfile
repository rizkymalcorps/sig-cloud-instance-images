FROM scratch
MAINTAINER rizky <rizky@detik.com>
ADD c68-docker.tar.xz /
LABEL name="CentOS Base Image" \
    vendor="CentOS" \
    license="GPLv2" \
    build-date="2018-01-02"
   
WORKDIR /tmp

RUN wget -q http://johnvansickle.com/ffmpeg/releases/ffmpeg-release-64bit-static.tar.xz \
  && tar xJf /tmp/ffmpeg-release-64bit-static.tar.xz -C /tmp \
  && mv /tmp/ffmpeg-3.0-64bit-static/ffprobe /usr/local/bin/ \
  && rm -rf /tmp/ffmpeg*

CMD ["--help"]
ENTRYPOINT ["ffprobe"]
