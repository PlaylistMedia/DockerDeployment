FROM golang:1.18.1-bullseye

RUN mkdir -p /backend
COPY ./PLBackend /backend
WORKDIR /backend

ENV PORT=3000

RUN go install github.com/cosmtrek/air@latest
CMD ["air"]


