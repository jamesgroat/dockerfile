FROM jetbrains/teamcity-agent:2021.2.3-linux-sudo

USER root
ENV TZ=America/Phoenix
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

RUN curl -sL https://deb.nodesource.com/setup_16.x | sudo -E bash -
RUN apt-get update -qq && apt-get install -qq -y build-essential nodejs
RUN npm install -g npm@latest

RUN curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip" && unzip awscliv2.zip && sudo ./aws/install
RUN curl -sL https://sentry.io/get-cli/ | bash

USER buildagent
