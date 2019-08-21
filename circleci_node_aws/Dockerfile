FROM circleci/node:10
RUN sudo apt-get update -qq && sudo apt-get install -y postgresql python-pip python-dev build-essential
RUN sudo pip install awscli
RUN sudo curl -sL https://sentry.io/get-cli/ | bash
