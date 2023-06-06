# BUILD FOR PRODUCTION
FROM node:18.15.0-alpine AS build

WORKDIR /usr/src/app

COPY . .

RUN npm ci

# TODO: uncomment when any models is defined in src/prisma/schema.prisma
# RUN npx prisma generate

ENV NODE_ENV production

RUN npm run build

RUN npm ci --omit=dev

# PRODUCTION
FROM node:18.15.0-alpine AS production

WORKDIR /usr/src/app

COPY --from=build /usr/src/app/node_modules ./node_modules

COPY --from=build /usr/src/app/dist ./dist

CMD [ "node", "dist/main" ]
