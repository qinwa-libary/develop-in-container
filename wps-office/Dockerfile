FROM lscr.io/linuxserver/wps-office:latest
ENV DISPLAY=:0.0
RUN \
    echo "**** install packages ****" && \
    apt-get update && \
    apt-get install --no-install-recommends -y \
    git \
    python3-venv \
    python3-pip \
    qtbase5-dev && \
    echo "**** cleanup ****" && \
    apt-get autoclean && \
    rm -rf \
    /var/lib/apt/lists/* \
    /var/tmp/* \
    /tmp/* 

COPY /fonts/ /usr/share/fonts/wps-fonts/

RUN fc-cache -vf
RUN git config --global --add safe.directory /com.docker.devenvironments.code

VOLUME /config