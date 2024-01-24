FROM golang:1.16

EXPOSE 8080

COPY . /usr/src/backend-app

WORKDIR /usr/src/backend-app

RUN go build

CMD [ "./server" ]