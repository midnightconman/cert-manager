FROM alpine:3.7

RUN apk add --no-cache ca-certificates

ADD cert-manager-acmesolver_linux_arm64 /usr/bin/acmesolver

ENTRYPOINT ["/usr/bin/acmesolver"]
ARG VCS_REF
LABEL org.label-schema.vcs-ref=$VCS_REF \
      org.label-schema.vcs-url="https://github.com/jetstack/cert-manager" \
      org.label-schema.license="Apache-2.0"
