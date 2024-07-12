FROM node:alpine
WORKDIR /app
# RUN addgroup dev && adduser -S -G dev daniel
# USER daniel
COPY . .

RUN apk add --no-cache python3 g++ make
RUN yarn install --production
CMD ["node","src/index.js"]

ENV API_URL=https://teste.com/api/v1
EXPOSE 3000