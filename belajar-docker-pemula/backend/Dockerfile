FROM golang:1.16-alpine

WORKDIR /app

COPY . .

RUN go build -o todolist-api

EXPOSE 8080

CMD ["./todolist-api"]