FROM mcr.microsoft.com/vscode/devcontainers/base:alpine

RUN apk update && apk add curl fish tar

ARG GO_VERSION=1.21.1
RUN curl -fsSL "https://go.dev/dl/go${GO_VERSION}.linux-amd64.tar.gz" | tar -xz -C /usr/local
ENV PATH $PATH:/usr/local/go/bin

RUN apk add gcc

USER vscode