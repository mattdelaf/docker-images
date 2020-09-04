# Python with yarn/nodejs.
# Note: python image has the libpq-dev by default.
FROM python:3.7

LABEL maintainer="Matthieu De La Fourniere<matthieudelafourniere@gmail.com>"
LABEL description="Available on DockerHub at mastymattdelaf/python-yarn"

RUN curl -sL https://deb.nodesource.com/setup_12.x | bash -
RUN curl -sL https://dl.yarnpkg.com/debian/pubkey.gpg | apt-key add -
RUN echo "deb https://dl.yarnpkg.com/debian/ stable main" | tee /etc/apt/sources.list.d/yarn.list
RUN apt-get update \
    && apt-get install -y nodejs yarn \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*