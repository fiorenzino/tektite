FROM golang:1.22

WORKDIR /usr/src/app

COPY . .
RUN make build-docker-full
RUN go build -o bin ./...

CMD ["bin/tektited","--config","cfg/standalone.conf"]
