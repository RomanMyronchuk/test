FROM node:18-alpine AS builder

WORKDIR /usr/src/app

# COPY *.json /usr/src/app

# RUN npm install

COPY . /usr/src/app

#RUN npm run build

# FROM node:18-alpine AS runner

# WORKDIR /app

# COPY --from=builder /app/node_modules ./node_modules

# COPY --from=builder /app/dist ./dist

# COPY --from=builder /app/*.json ./

# Виставляємо змінні середовища (при необхідності)
ARG NODE_ENV=dev

ENV NODE_ENV=$NODE_ENV
# ENV NODE_ENV=dev

EXPOSE 3001

CMD sh -c "node index.js"
