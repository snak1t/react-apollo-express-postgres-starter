FROM node:carbon

WORKDIR /usr/src/app
COPY . .

RUN npm install
RUN npm install pm2 -g
RUN npm install cross-env -g

EXPOSE 3100
CMD ["pm2-runtime", "process.yml"]
