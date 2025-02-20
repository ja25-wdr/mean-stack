FROM node:22.11.0

WORKDIR /app

COPY package*.json /app


RUN npm install -g @angular/cli

RUN npm install

COPY . .

CMD ["ng", "serve", "--host", "0.0.0.0"]