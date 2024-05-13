ARG VARIANT=ubuntu-22.04
FROM mcr.microsoft.com/vscode/devcontainers/base:0-${VARIANT} as base


FROM base as devcontainer

RUN <<EOF
  apt update
  apt install git make python3-pip -y
  pip3 install ansible
  apt clean
EOF