FROM alpine:latest

RUN apk add --update && \
    apk add yq && \
    rm /var/cache/apk/*

COPY --from=alpine/helm:latest /usr/bin/helm /usr/bin/helm
RUN chmod +x /usr/bin/helm

CMD []
