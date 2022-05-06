FROM debian

LABEL maintainer=@abel-losada
ARG DEBIAN_FRONTEND=noninteractive

ENV LANG=C.UTF-8 LC_ALL=C.UTF-8
ENV PATH /opt/conda/bin:$PATH

RUN apt-get update --fix-missing && \
  apt-get install -y \
  wget bzip2 ca-certificates \
  libglib2.0-0 libxext6 libsm6 libxrender1

RUN wget --quiet \
  https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh -O ~/miniconda.sh && \
  /bin/bash ~/miniconda.sh -b -p /opt/conda && \
  rm ~/miniconda.sh