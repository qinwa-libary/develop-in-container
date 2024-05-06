FROM docker/dev-environments-default:stable-1

WORKDIR /tmp

RUN \
    echo "**** install packages ****" && \
    apt-get update && \
    apt-get install --no-install-recommends -y \
    openjdk-17-jdk \
    maven && \
    echo "**** cleanup ****" && \
    apt-get autoclean && \
    rm -rf \
    /var/lib/apt/lists/* \
    /var/tmp/* \
    /tmp/*
