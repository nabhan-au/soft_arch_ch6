FROM node:18.7.0

ARG port=3000

ENV PORT=${port}

WORKDIR /usr/src/app/

COPY ./package*.json ./

RUN npm install --only=production

COPY ./ ./

EXPOSE ${port}

CMD [ "npm", "start" ]

