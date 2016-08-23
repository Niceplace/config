FROM python:alpine

RUN mkdir /downloads
VOLUME /downloads
RUN apk add --update py-pip ffmpeg
RUN pip install --upgrade youtube_dl

ENTRYPOINT [ "youtube-dl" ]
