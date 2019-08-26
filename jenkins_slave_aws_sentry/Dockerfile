FROM jenkins/slave:3.29-2

USER root
RUN apt-get update -qq && apt-get install -y postgresql python-pip python-dev build-essential
USER jenkins

RUN pip install awscli
RUN curl -sL https://sentry.io/get-cli/ | bash

COPY jenkins-slave /usr/local/bin/jenkins-slave

ENTRYPOINT ["jenkins-slave"]

