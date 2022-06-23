FROM debian:buster-slim

# Disable prompts from apt.
ENV DEBIAN_FRONTEND noninteractive

RUN apt-get -qq update && \
    apt-get -qq --no-install-recommends --no-install-suggests --yes --quiet install \
        curl \
        ca-certificates \
        jq && \
    apt-get --yes autoremove --purge && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

CMD ["tail", "-F", "-n0", "/etc/hosts" ]
