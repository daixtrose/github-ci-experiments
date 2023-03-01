ARG BASE_IMAGE
FROM $BASE_IMAGE

RUN apt-get update \
    && DEBIAN_FRONTEND="noninteractive" apt-get install -y --no-install-recommends \
    lsb-release \
    pkg-config \
    ubuntu-desktop \
    firefox \
    xrdp \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

# firefox
# sudo apt -y install xrdp
# sudo adduser xrdp ssl-cert
# //sudo systemctl restart xrdp

# sudo ufw allow 3389
