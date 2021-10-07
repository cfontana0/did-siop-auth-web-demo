FROM node:14

COPY .. .
RUN yarn global add ts-node
RUN yarn install

ENTRYPOINT ["yarn", "start"]
