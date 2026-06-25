FROM ubuntu:24.04

RUN groupadd -g 1001 user && \
    useradd -m -s /bin/bash -u 1001 -g 1001 user 

RUN apt-get update && \
    apt-get install -y --no-install-recommends \
    ca-certificates \
    jq \
    bash \
    curl \
    unzip \
    python3 \
    python3-pip \
    python3-venv \
    && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*

USER 1001
