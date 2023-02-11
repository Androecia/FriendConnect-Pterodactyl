FROM        bitnami/node:18

LABEL       author="Loki" maintainer="loki@crazycoder.dev"

WORKDIR     /mnt
RUN         apt update\
            && apt -y install git cmake\
            && git clone https://github.com/Androecia/FriendConnect.git
WORKDIR     /mnt/FriendConnect

RUN         npm install npm@latest -g\
            && npm i\
            && npm run build