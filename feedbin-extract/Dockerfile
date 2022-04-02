FROM alpine:3.13

WORKDIR /app

RUN apk add --no-cache \
    git \
    nodejs \
    npm \
    && git clone https://github.com/feedbin/extract.git /app \
    && npm ci \
    && mkdir users

CMD ["node", "app/server.js"]
