FROM alpine:3.24.3

RUN addgroup -g 1001 user && \
    adduser -D -s /bin/sh -u 1001 -G user user

RUN apk add --no-cache \
    ca-certificates \
    curl \
    age && \
    rm -rf /var/cache/apk/*

USER 1001
