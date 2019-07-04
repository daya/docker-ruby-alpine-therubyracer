FROM ruby:2.6.3-alpine3.10
ENV LIBV8_VERSION 7.3.492.27.1
RUN apk add --update --no-cache libstdc++ && \
    apk add --update --no-cache --virtual build-deps build-base make python git bash && \
    gem install libv8 -v ${LIBV8_VERSION} && \
    gem install therubyracer && \
    apk del build-deps
