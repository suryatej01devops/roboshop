FROM almalinux:9

RUN dnf -y update && \
    dnf -y remove curl-minimal && \
    dnf -y install \
        curl \
        iputils \
        iproute \
        traceroute \
        telnet \
        bind-utils && \
    dnf clean all && \
    rm -rf /var/cache/dnf

CMD ["sleep","100000"]