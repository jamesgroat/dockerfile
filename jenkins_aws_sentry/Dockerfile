FROM jenkins/jenkins:lts

USER root
RUN apt-get update -qq && apt-get install -y postgresql python-pip python-dev build-essential
RUN pip install awscli
RUN curl -sL https://sentry.io/get-cli/ | bash

USER jenkins

