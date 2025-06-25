FROM golang:1.20-alpine
RUN apk add --no-cache curl
WORKDIR /app
COPY . .
RUN go build -o app main.go
EXPOSE 8001
CMD ["./app"]

