FROM node:17-alpine

RUN mkdir -p /frontend
COPY ./Playlist /frontend
WORKDIR /frontend

ENV PORT=3000

RUN npm install
CMD ["npm", "start"]

