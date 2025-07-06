FROM node:20-alpine AS base

WORKDIR /app

COPY src/web/package*.json ./

RUN npm install 

COPY ./src/web/ .

EXPOSE 59171

CMD ["npm", "run", "dev", "--", "--host", "0.0.0.0"]
