FROM nvidia/cuda:12.2.2-cudnn8-runtime-ubuntu22.04

RUN apt-get -y update \
    && apt-get install -y software-properties-common \
    && apt-get -y update

COPY /root/ /root

WORKDIR /root
