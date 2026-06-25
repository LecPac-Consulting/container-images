FROM ghcr.io/lecpac-consulting/container-images/base:stable

USER root

RUN apt-get update && \
    apt-get install -y --no-install-recommends cryptsetup mdadm xfsprogs fio && \
    rm -rf /var/lib/apt/lists/*

USER 1001
