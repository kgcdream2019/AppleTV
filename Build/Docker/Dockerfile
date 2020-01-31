# Build stage
FROM ubuntu:18.04

RUN echo ========== Install dependencies ========== \
  && apt-get update && apt-get install -y \
    clang \
    git \
    make \
    perl \
    unzip \
    wget \
    libavahi-compat-libdnssd-dev \
    libssl-dev \
    openssh-server \
  && rm -rf /var/lib/apt/lists/*

RUN apt-get update && apt-get install -y gdb

WORKDIR /build
