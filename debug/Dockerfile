FROM almalinux:9
RUN dnf -y update && \
    dnf -y install \
        iputils \
        iproute \
        traceroute && \
    dnf clean all && \
    rm -rf /var/cache/dnf
CMD ["sleep","100000"]