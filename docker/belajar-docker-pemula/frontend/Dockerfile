FROM node:14-alpine

WORKDIR /app

ENV VUE_APP_API_URL=http://localhost:8080
ENV YARN_IGNORE_ENGINES=1

# copy dependency descriptor dulu (biar cache bener)
COPY package.json ./

# install dependency sesuai lock lama
RUN yarn install --force --no-progress

# copy source code
COPY . .

EXPOSE 8080

CMD ["yarn", "serve"]
