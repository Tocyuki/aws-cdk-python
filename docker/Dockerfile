# the latest Python
FROM python:latest

# install the latest nodejs & npm
RUN apt update \
 && apt install -y nodejs npm \
 && apt clean

# install the latest AWS CDK & AWSCLI
RUN npm install -g aws-cdk \
&& pip3 install --upgrade aws-cdk.core \
&& pip3 install awscli --upgrade

ENTRYPOINT [ "/usr/local/bin/cdk" ]
