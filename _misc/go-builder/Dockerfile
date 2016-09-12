FROM alpine:edge
RUN apk --update add bash go bzr git mercurial subversion openssh-client ca-certificates gcc linux-headers build-base
RUN mkdir -p /go/src /go/bin && chmod -R 777 /go
ENV GOPATH /go
ENV PATH /go/bin:$PATH
WORKDIR /go


