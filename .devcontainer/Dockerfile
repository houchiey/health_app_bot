FROM mcr.microsoft.com/devcontainers/typescript-node:0-18

RUN apt-get update \
    && apt-get -y install --no-install-recommends apt-utils dialog 2>&1 \
    && apt-get -y install git \
    && curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py \
    && python3 get-pip.py \
    && rm get-pip.py \
    && pip install awscli \
    && npm install -g aws-cdk \
    && pip install aws-sam-cli
