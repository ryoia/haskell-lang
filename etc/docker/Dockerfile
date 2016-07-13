# Dockerfile for fpco/haskell-lang-base
#-*- mode: conf; -*-

FROM ubuntu:14.04
ENV LANG=C.UTF-8
RUN apt-get update \
 && apt-get install -y --no-install-recommends libgmp10 ca-certificates libicu-dev \
 && apt-get clean
COPY haskell-lang /usr/local/bin/haskell-lang
COPY config/ /haskell-lang/config/
COPY static/ /haskell-lang/static/
COPY themes/ /haskell-lang/themes/
CMD haskell-lang
