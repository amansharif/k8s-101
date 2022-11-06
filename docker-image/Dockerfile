# Start by building the application.
FROM golang:1.18 as build

RUN git clone https://github.com/amansharif/microservice-demo.git; \
    cd microservice-demo/application;

WORKDIR /go/microservice-demo/application

RUN go mod download
RUN CGO_ENABLED=0 go build

CMD ["./application"]