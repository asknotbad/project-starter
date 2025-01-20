FROM node:22-alpine AS builder

RUN mkdir -p /app
WORKDIR /app

COPY . .
RUN npm ci
RUN npm run build

FROM node:22-alpine

COPY --from=builder /app/package*.json ./
COPY --from=builder /app/node_modules ./node_modules
COPY --from=builder /app/build ./build

EXPOSE 3000

CMD [ "node", "build/index.js" ]
