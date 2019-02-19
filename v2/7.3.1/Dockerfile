FROM node:lts

ENV GITEMAIL=email@example.com
ENV GITUSER=SomeUser
ENV PORT=4200

RUN apt update && apt upgrade -y
RUN apt install bash git -y

WORKDIR /app

VOLUME ["/app"]

RUN npm install -g @angular/cli@7.3.1

EXPOSE 4200-4219

ADD start_script.sh /usr/local/bin/start_script
RUN chmod +x /usr/local/bin/start_script
RUN chmod -R 777 /app



