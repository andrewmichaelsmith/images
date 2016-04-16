FROM alpine:edge
RUN \
	echo "http://dl-cdn.alpinelinux.org/alpine/edge/testing" >> \
		/etc/apk/repositories && \
	apk add --update tor && \
	rm -rf /var/cache/apk/*
USER tor
ADD torrc /etc/tor/
CMD ["tor"]
