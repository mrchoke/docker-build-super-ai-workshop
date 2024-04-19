FROM golang

WORKDIR /app

COPY main.go .

ENV CGO_ENABLED 0
ENV GOOS linux 
ENV GOARCH ${TARGETARCH}

RUN go build -o hello main.go

CMD ["/app/hello"]