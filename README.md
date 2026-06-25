# Container Images

This repository contains images used in various contexts in LecPac Consulting or for its clients.

This provided is maintained by [LecPac Consulting](https://lecpac-consulting.com), a Managed Services Provider (MSP) based in France.
Images are automatically rebuilt every week.

Licensed under the [Apache-2.0](LICENSE) license.

## Available images

- `ghcr.io/lecpac-consulting/container-images/base:stable`: The image contains various tools useful in containerized environments, such as git, jq, bash, curl, python3 and pip.
- `ghcr.io/lecpac-consulting/container-images/toolkit-fs:stable`: The image contains all tools from `base` plus additional tools useful in filesystem operations: cryptsetup, mdadm, xfsprogs, fio.
- `ghcr.io/lecpac-consulting/container-images/mongosync:stable`: The image contains all tools from `base` plus [Mongosync](https://www.mongodb.com/docs/mongosync/current/).
