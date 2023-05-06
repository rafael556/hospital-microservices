FROM node:16-alpine
WORKDIR /app
COPY package.json ./
RUN yarn --production
COPY . .
RUN yarn build
EXPOSE 3000
CMD ["yarn", "start"]