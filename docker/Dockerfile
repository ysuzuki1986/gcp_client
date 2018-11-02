FROM ubuntu:18.04
USER root
RUN apt-get update && \
    apt-get install -y curl software-properties-common && \
    curl -L https://dl.google.com/dl/cloudsdk/channels/rapid/downloads/google-cloud-sdk-223.0.0-linux-x86_64.tar.gz -o /usr/local/google-cloud-sdk.tar.gz && \
    tar zxvf /usr/local/google-cloud-sdk.tar.gz -C /usr/local
ENV PATH /usr/local/google-cloud-sdk/bin/:$PATH
CMD /bin/bash
