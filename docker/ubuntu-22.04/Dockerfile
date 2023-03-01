ARG BASE_IMAGE
FROM $BASE_IMAGE

ENV DEBIAN_FRONTEND noninteractive

RUN apt-get update \
    && apt-get install -y --no-install-recommends \
    lsb-release \
    pkg-config \
    ubuntu-desktop \
    task-gnome-desktop \
    firefox \
    xrdp \
    net-tools \
    xorgxrdp \
    less \
    dbus-x11 \
    git \
    locales \
    pavucontrol \
    pulseaudio \
    pulseaudio-utils \
    sudo \
    x11-xserver-utils \
    xfce4 \
    xfce4-goodies \
    xfce4-pulseaudio-plugin \
    xorgxrdp \
    xubuntu-icon-theme \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*


# dbus-x11 war wohl nicht nötig
#  task-gnome-desktop?

# firefox
# sudo apt -y install xrdp
# sudo adduser xrdp ssl-cert
# //sudo systemctl restart xrdp

# sudo ufw allow 3389

COPY entrypoint.sh /usr/bin/entrypoint
ENTRYPOINT ["/usr/bin/entrypoint"]


