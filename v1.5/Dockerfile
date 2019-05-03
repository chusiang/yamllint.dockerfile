FROM python:3-alpine3.9

MAINTAINER Chu-Siang Lai <chusiang@drx.tw>

RUN echo "===> Update the index of available packages ..."  && \
      apk update

RUN echo "===> Install some package ..."  && \
      apk add --no-cache make

RUN echo "===> Install the yamllint ..."  && \
      pip install 'yamllint>=1.15.0,<1.16.0'

RUN echo "===> Removing package cache ..."  && \
      apk del build-dependencies             ; \
      rm -rf /var/cache/apk/*               && \
      rm -rf ~/.cache/pip

WORKDIR /srv

CMD [ "yamllint", "--version" ]
