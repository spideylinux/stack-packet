FROM BASEIMAGE
RUN apk --no-cache add ca-certificates bash

ARG ARCH
ARG TINI_VERSION

ADD stack /usr/local/bin/crossplane-packet-stack

COPY stack-package /

EXPOSE 8080
ENTRYPOINT ["crossplane-packet-stack"]