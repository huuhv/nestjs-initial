FROM node:18.15.0-alpine

ENV NODE_ENV development

WORKDIR /usr/src/app

COPY . .

RUN npm install

# TODO: uncomment when any models is defined in src/prisma/schema.prisma
# RUN npx prisma generate

CMD [ "npm", "run", "start:dev" ]
