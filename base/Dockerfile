FROM debian:jessie
LABEL maintainer="apds.anderson@gmail.com"

WORKDIR /app/

RUN apt-get update -qy \
    && apt-get install -qy cmake build-essential libboost-all-dev git ca-certificates --no-install-recommends
