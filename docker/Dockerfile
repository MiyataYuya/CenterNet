FROM nvcr.io/nvidia/pytorch:23.04-py3

RUN apt update && apt upgrade -y

ARG USERNAME=miyata
ARG GROUPNAME=miyata
ARG UID=1000
ARG GID=1000
RUN groupadd -g $GID $GROUPNAME && \
    useradd -m -s /bin/bash -u $UID -g $GID $USERNAME
USER $USERNAME