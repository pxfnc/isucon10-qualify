FROM python:3

WORKDIR /workdir

RUN set -ex && \
    cd /tmp && \
    curl -O https://dl.google.com/go/go1.16.7.linux-amd64.tar.gz && \
    tar -C /usr/local -xzf go1.16.7.linux-amd64.tar.gz && \
    rm /tmp/go1.16.7.linux-amd64.tar.gz


COPY . . 

ENV PATH $PATH:/usr/local/go/bin
