# Dockerfile for the module tutorial and coursework
# minimum

FROM ubuntu:20.04

# git and conda
RUN apt-get update && apt-get install -y wget git \
 && rm -rf /var/lib/apt/lists/*
RUN wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh \
 && mkdir /root/.conda \
 && bash Miniconda3-latest-Linux-x86_64.sh -b \
 && rm -f Miniconda3-latest-Linux-x86_64.sh
ARG PATH="/root/miniconda3/bin:$PATH"
RUN conda init bash
ENV PATH="/root/miniconda3/bin:$PATH"
