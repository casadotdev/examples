FROM ruby:3.2.2


RUN apt-get update -y \
    && apt-get install -y --no-install-recommends \
    && rm -rf /var/lib/apt/lists/*

COPY /root/ /root

WORKDIR /root

RUN bundle install

