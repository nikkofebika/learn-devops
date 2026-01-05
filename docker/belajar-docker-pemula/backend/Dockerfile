FROM golang:1.16-alpine

WORKDIR /app

COPY . .

RUN go build -o todolist-api

# VOLUME [ "/data" ]

EXPOSE 8080

CMD ["./todolist-api"]