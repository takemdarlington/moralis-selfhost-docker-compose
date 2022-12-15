FROM node:18-alpine

WORKDIR /usr/src/app

EXPOSE 1337
# COPY --chown=node:node package*.json ./
COPY package*.json ./

RUN yarn

COPY . .

RUN yarn build

# COPY --chown=node:node . .

# USER node

CMD ["yarn", "dev"]