FROM debian:jessie
#FROM ubuntu:18.04

MAINTAINER rohit.gabriel@enterpriseit.co.nz

# image: customrepo/docker-builder



RUN apt-get update -y

RUN apt-get install -y curl ssh-client





# docker

ENV DOCKER_BUCKET get.docker.com

ENV DOCKER_VERSION 17.12.1-ce



RUN set -x \

	&& curl -fSL "https://download.docker.com/linux/static/stable/x86_64/docker-${DOCKER_VERSION}.tgz" -o docker.tgz \

	&& tar -xzvf docker.tgz \

	&& mv docker/* /usr/local/bin/ \

	&& rmdir docker \

	&& rm docker.tgz \

	&& docker -v





CMD top
