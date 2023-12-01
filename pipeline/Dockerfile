FROM golang:1.21

WORKDIR /app/server

COPY server ./ 
RUN go mod download

RUN CGO_ENABLED=0 GOOS=linux go build

EXPOSE 8080

CMD ./server
