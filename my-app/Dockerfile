# syntax=docker/dockerfile:1
FROM node:18-alpine
WORKDIR /my-app
COPY . .
RUN npm ci
RUN npm run build
ENV NODE_ENV production
EXPOSE 3000
CMD ["npm", "start", "build"]