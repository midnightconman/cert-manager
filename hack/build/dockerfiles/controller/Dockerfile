FROM alpine:3.7

RUN apk add --no-cache ca-certificates

ADD cert-manager-controller_linux_arm64 /usr/bin/cert-manager

ENTRYPOINT ["/usr/bin/cert-manager"]
ARG VCS_REF
LABEL org.label-schema.vcs-ref=$VCS_REF \
      org.label-schema.vcs-url="https://github.com/jetstack/cert-manager" \
      org.label-schema.license="Apache-2.0"
