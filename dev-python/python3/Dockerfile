FROM docker/dev-environments-default:stable-1

RUN \
    echo "**** install packages ****" && \
    apt-get update && \
    apt-get install --no-install-recommends -y \
    python3-venv \
    python3-pip && \
    echo "**** cleanup ****" && \
    apt-get autoclean && \
    rm -rf \
    /var/lib/apt/lists/* \
    /var/tmp/* \
    /tmp/* 