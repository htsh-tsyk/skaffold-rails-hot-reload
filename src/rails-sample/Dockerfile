FROM ruby:2.7.1

# install dependencies
RUN apt-get update -qq && \
    apt-get install -y build-essential libpq-dev

RUN mkdir /app
WORKDIR /app

ADD Gemfile /app/Gemfile
ADD Gemfile.lock /app/Gemfile.lock
RUN bundle install
ADD . /app


RUN mkdir -p tmp/sockets

CMD bundle exec puma
