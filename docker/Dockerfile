FROM golang:1.22

WORKDIR /usr/src/app

COPY . .
RUN go build -o bin ./...
ENV PATH="${PATH}:/usr/src/app/bin"

EXPOSE 44400 7770 8880 9990 

CMD tektited --config /usr/src/app/cfg/standalone.conf
