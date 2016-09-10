FROM alpine:edge
RUN \
       apk update && \
       apk add ca-certificates && \
	   apk add openssl && \
       update-ca-certificates && \
       wget https://github.com/prometheus/prometheus/releases/download/v1.1.2/prometheus-1.1.2.linux-amd64.tar.gz && \
       tar xfzv prometheus-1.1.2.linux-amd64.tar.gz && \
       mv prometheus-1.1.2.linux-amd64/prometheus /usr/local/bin/ && \
       rm -rf prometheus-1.1.2.linux-amd64*

ENTRYPOINT ["/prometheus-1.1.2.linux-amd64/prometheus"]

