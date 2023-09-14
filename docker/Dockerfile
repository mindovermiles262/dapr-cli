FROM alpine

ARG VERSION=1.11.0
ARG ARCH=linux
ARG CPU=amd64

RUN apk add wget
RUN wget \
    --quiet \
    -O dapr-cli.tgz \
    https://github.com/dapr/cli/releases/download/v${VERSION}/dapr_${ARCH}_${CPU}.tar.gz \
  && tar -xf dapr-cli.tgz \
  && rm dapr-cli.tgz \
  && mv dapr /bin/dapr
