FROM ubuntu:20.04

ENV DEBIAN_FRONTEND=noninteractive

RUN \
  apt-get update && \
  apt-get install -y git-core nginx fcgiwrap curl && \
  rm -rf /var/lib/apt/lists/*

COPY entrypoint /
ENTRYPOINT ["/entrypoint"]
