# Version 1.0.0
# Yves Vindevogel
# 2018-08-13
FROM debian:stretch-slim

MAINTAINER Yves Vindevogel (yves.vindevogel@asynchrone.com)

ENV SHELL=/bin/bash

ARG DEBIAN_FRONTEND=noninteractive
ARG TIMEZONE="Europe/Brussels"

RUN apt-get update --yes
RUN apt-get upgrade --yes

RUN echo $TIMEZONE > /etc/timezone

RUN apt-get autoremove --yes
RUN apt-get clean
RUN rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

CMD [ "/bin/bash" ]
