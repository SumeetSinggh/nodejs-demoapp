FROM node:lts-alpine3.21

WORKDIR /app
COPY /src/package.json .
COPY /src/package-lock.json .

RUN npm install --production --silent

COPY src/ .

EXPOSE 3000
CMD npm start