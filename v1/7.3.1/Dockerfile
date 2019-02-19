FROM node:lts


RUN apt update && apt upgrade -y
RUN apt install bash git -y

WORKDIR /app

VOLUME ["/app"]

RUN npm install -g @angular/cli:7.3.1

EXPOSE 4200

ADD start_script.sh /usr/local/bin/start_script.sh



