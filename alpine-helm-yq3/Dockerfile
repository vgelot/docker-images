FROM alpine:latest

COPY --from=mikefarah/yq:3.3.1 /usr/bin/yq /usr/bin/yq
RUN chmod +x /usr/bin/yq

COPY --from=alpine/helm:latest /usr/bin/helm /usr/bin/helm
RUN chmod +x /usr/bin/helm

CMD []
