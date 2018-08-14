# Version 1.0.0

FROM debian:stretch-slim

MAINTAINER Yves Vindevogel (yves.vindevogel@asynchrone.com)

ENV SHELL=/bin/bash

ARG DEBIAN_FRONTEND=noninteractive
ARG TIMEZONE="Europe/Brussels"

COPY ./bashrc /root/.bashrc

RUN apt-get update --yes
RUN apt-get upgrade --yes

RUN apt-get install apt-utils --yes --no-install-recommends

RUN echo $TIMEZONE > /etc/timezone

RUN apt-get autoremove --yes
RUN apt-get clean
RUN rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

CMD [ "/bin/bash" ]
