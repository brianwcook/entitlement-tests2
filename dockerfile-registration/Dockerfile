FROM registry.access.redhat.com/ubi9/ubi
USER 0
RUN subscription-manager register --org $(cat "/activation-key/org") --activationkey $(cat "/activation-key/activationkey")
RUN dnf -y install golang kernel-devel
RUN subscription-manager unregister
