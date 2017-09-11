FROM node:8

RUN apt-get update --yes \
  && apt-get install --yes \
    libgtk2.0-0 \
    libnotify-dev \
    libgconf-2-4 \
    libnss3 \
    libxss1 \
    xvfb

RUN npm install -g cypress-cli \
  && cypress install && cypress verify

ENTRYPOINT ["bash"]
