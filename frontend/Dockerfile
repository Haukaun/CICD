FROM node:14-alpine

WORKDIR /frontend

COPY package.json .
COPY package-lock.json .
RUN npm install
RUN npm install -g serve

COPY . . 

EXPOSE 3000

CMD npm run build && serve -s build
