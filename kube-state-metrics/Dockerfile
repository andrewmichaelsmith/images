FROM alpine:edge
RUN apk --update add ca-certificates openssl && \
    update-ca-certificates && \
    wget https://github.com/andrewmichaelsmith/images/raw/master/kube-state-metrics/kube-state-metrics -O /usr/local/bin/kube-state-metrics
ENTRYPOINT ["/usr/local/bin/kube-state-metrics"]
