FROM golang

COPY . /go/src

WORKDIR /go/src

RUN go mod download

RUN go build -o /go/bin/test .

#CMD ["/bin/sh", "/go/src/.ops/wait.sh"]

CMD ["/go/bin/test"]