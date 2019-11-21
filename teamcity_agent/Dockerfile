FROM jetbrains/teamcity-agent

RUN curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -
RUN apt-get update -qq && apt-get install -qq -y postgresql python-pip python-dev build-essential nodejs
RUN pip install awscli
RUN curl -sL https://sentry.io/get-cli/ | bash
