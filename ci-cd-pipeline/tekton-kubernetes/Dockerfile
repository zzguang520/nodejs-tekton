FROM node:12.16-alpine

ADD bin          /app/bin
ADD public       /app/public
ADD routes       /app/routes
ADD views        /app/views
ADD app.js       /app/
ADD package.json /app/

RUN ls -l /app

RUN cd /app && npm install

EXPOSE  8080

CMD ["node", "/app/bin/www"]