FROM node:18-slim

RUN apt-get update && apt-get install -y git

WORKDIR /app

COPY package*.json ./
RUN npm install

COPY . .

EXPOSE 5173
CMD ["npm", "run", "dev"]
