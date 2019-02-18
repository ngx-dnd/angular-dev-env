FROM node:lts

ENV gitEmail=email@example.com
ENV gitUser=SomeUser

RUN apt update && apt upgrade -y
RUN apt install bash git -y

WORKDIR /app

VOLUME ["/app"]

RUN npm install -g @angular/cli

EXPOSE 4200

ADD start_script.sh /usr/local/bin/start_script.sh

CMD [ "/usr/local/bin/start_script.sh" ]

