# -- DEV DOCKERFILE --
# -- DO NOT USE IN PRODUCTION! --

FROM node:20
LABEL maintainer "requarks.io"

RUN apt-get update && \
    apt-get install -y bash curl git python3 make g++ nano openssh-server gnupg && \
    mkdir -p /wiki && \
    apt-get clean

WORKDIR /wiki

ENV dockerdev 1
ENV DEVDB postgres

EXPOSE 3000

CMD ["tail", "-f", "/dev/null"]
