FROM node:17-alpine

RUN mkdir -p /frontend
COPY ./testing /frontend
WORKDIR /frontend

ENV PORT=4000

RUN npm install
CMD ["npm", "start"]

