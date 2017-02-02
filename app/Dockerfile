FROM node:6.9

MAINTAINER Alfonso Rodriguez <beabys@gmail.com>

ADD ./ ./
RUN npm install pm2 -g
RUN npm install --save

EXPOSE 3000

CMD ["pm2-docker", "./bin/www"]