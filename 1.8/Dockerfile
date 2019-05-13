FROM elixir:1.8.1
MAINTAINER Edwin Mak <edwinthinks@gmail.com>

RUN apt-get update -y \ 
 && apt-get install -y curl \
 && curl -sL https://deb.nodesource.com/setup_10.x | bash \
 && apt-get install -y apt-utils \
 && apt-get install -y nodejs \
 && apt-get install -y build-essential \
 && apt-get install -y inotify-tools

# Install Rebase + Hex
RUN mix local.hex --force \
  && mix local.rebar --force


