FROM python:3.13-alpine3.21

LABEL org.opencontainers.image.authors="chusiang@drx.tw"

RUN echo "===> Update the index of available packages ..."  && \
  apk update

RUN echo "===> Install some package ..."    && \
  apk add --no-cache make

ENV PIP_ROOT_USER_ACTION=ignore

RUN echo "===> Install the yamllint ..."    && \
  pip install --no-cache-dir 'yamllint>=1.37.0,<1.38.0'

RUN echo "===> Removing package cache ..."  && \
  rm -rf /var/cache/apk/*                   && \
  rm -rf ~/.cache/pip

WORKDIR /srv

CMD [ "yamllint", "--version" ]
