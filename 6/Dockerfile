FROM node:boron

LABEL maintainer "Spencer Thornock <spencer.thornock@gmail.com>"

USER root

RUN mkdir /home/.npm-global
ENV PATH=/home/.npm-global/bin:$PATH
ENV NPM_CONFIG_PREFIX=/home/.npm-global

# Install node dependencies
RUN npm install --quiet --no-progress -g firebase-tools
RUN npm cache clean --force
