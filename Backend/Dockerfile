FROM golang:1.18.1-alpine3.15

RUN mkdir -p /backend
COPY ./PLBackend /backend
WORKDIR /backend

ENV PORT=3000

RUN apk update
RUN apk add git
RUN go install github.com/cosmtrek/air@latest
RUN go mod download && go mod verify

CMD ["air", "-c", ".air.toml"]

