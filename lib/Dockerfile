FROM node:lts-buster

RUN git clone https://github.com/Lokixgod75/new/ /root/Lokixgod75

WORKDIR /root/Lokixgod75

RUN apt-get update && \
  apt-get install -y \
  ffmpeg \
  imagemagick \
  webp && \
  apt-get upgrade -y && \
  rm -rf /var/lib/apt/lists/*

RUN npm install


CMD ["npm", "index.js"]
