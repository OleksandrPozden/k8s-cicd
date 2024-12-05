# Stage-1 & spacify a name 'builder'
FROM  node:latest AS builder

WORKDIR /app

COPY package.json .
RUN npm install

COPY . .

RUN npm run build

# Stage-2
FROM nginx:1.25.2-alpine-slim

EXPOSE 80

COPY --from=builder /app/build /usr/share/nginx/html
COPY ./nginx/default-prod.conf /etc/nginx/conf.d/default.conf