FROM debian

LABEL version=1.0
LABEL description ="this image containe nodejs"

RUN apt upgrade && apt update -y

RUN apt -y install build-essential
RUN apt -y install curl dirmngr apt-transport-https lsb-release ca-certificates
RUN curl -sL https://deb.nodesource.com/setup_12.x | bash -

RUN apt install nodejs -y

RUN apt install git -y

RUN npm install -g typescript
RUN npm install -g @vue/cli @vue/cli-service-global
RUN npm install -g @angular/cli

WORKDIR /var/www

CMD tail -f /dev/null