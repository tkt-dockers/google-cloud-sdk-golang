FROM google/cloud-sdk:291.0.0

LABEL maintainer="tktcorporation <tktcorporation@gmail.com>"

ENV GOPATH /go
ENV PATH $GOPATH/bin:/usr/local/bin:$PATH

ENV GOLANG_VERSION 1.12.17

RUN curl -Lso go.tar.gz "https://dl.google.com/go/go${GOLANG_VERSION}.linux-amd64.tar.gz" \
    && tar -C /usr/local -xzf go.tar.gz \
    && rm go.tar.gz

ENV PATH /usr/local/go/bin:$PATH

RUN go get -u github.com/golang/dep/cmd/dep