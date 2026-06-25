FROM ghcr.io/lecpac-consulting/container-images/base:stable

USER root

ARG MONGOSYNC_VERSION=1.20.0
RUN curl -O https://fastdl.mongodb.org/tools/mongosync/mongosync-ubuntu2404-x86_64-${MONGOSYNC_VERSION}.tgz \
        && echo "bcfb14e5c553bf1f63d4687c5679f30c0bb7058051b5b55e6cfe5d35de61b9c8  mongosync-ubuntu2404-x86_64-${MONGOSYNC_VERSION}.tgz" | sha256sum -c - \
        && tar -xzf mongosync-ubuntu2404-x86_64-${MONGOSYNC_VERSION}.tgz \
        && cp mongosync-ubuntu2404-x86_64-${MONGOSYNC_VERSION}/bin/mongosync /usr/local/bin/ \
        && rm -rf /var/lib/apt/lists/*

USER 1001
