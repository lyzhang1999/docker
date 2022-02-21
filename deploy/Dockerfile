FROM ubuntu:latest

RUN apt-get update && apt-get install curl -y && apt-get install git -y && curl -LO https://dl.k8s.io/release/v1.23.4/bin/linux/$(dpkg --print-architecture)/kubectl && chmod +x kubectl && mv kubectl /usr/local/bin/kubectl  && apt-get clean

RUN curl https://raw.githubusercontent.com/helm/helm/main/scripts/get-helm-3 | bash