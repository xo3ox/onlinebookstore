FROM golang:latest
RUN go env -w GO111MODULE=on
RUN go env -w GOPROXY=https://goproxy.cn,https://goproxy.io,direct

WORKDIR $GOPATH/src/onlinebookstore
COPY . $GOPATH/src/onlinebookstore

RUN go build .

EXPOSE 3000

ENTRYPOINT ["./onlinebookstore"]