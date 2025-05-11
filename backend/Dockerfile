FROM node:20-alpine AS base
# ARG DATAbase_URL

WORKDIR /usr/src/app
COPY package*.json ./
RUN npm install

FROM base AS development
COPY . .
EXPOSE 3000
CMD ["node","index.js"]
