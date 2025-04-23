FROM node:22.11.0

WORKDIR /app

# Copy package.json and package-lock.json for dependency installation
COPY package*.json ./

RUN npm install -g @angular/cli

RUN npm install

# Copy the application code into the container
COPY . .

CMD ["ng", "serve", "--host", "0.0.0.0"]