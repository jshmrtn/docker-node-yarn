FROM jshmrtn/node-yarn:6.9.1

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

ONBUILD ARG NODE_ENV
ONBUILD ENV NODE_ENV $NODE_ENV
ONBUILD COPY package.json /usr/src/app/
ONBUILD RUN yarn install
ONBUILD COPY . /usr/src/app

CMD [ "yarn", "start" ]
