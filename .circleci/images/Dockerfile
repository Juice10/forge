# Use base docker image for docker builder
FROM snapcore/snapcraft

# Install dependencies for docker builder
RUN add-apt-repository -y ppa:alexlarsson/flatpak
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 536F8F1DE80F6A35
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 4EB27DB2A3B88B8B
RUN apt-get update
RUN apt-get dist-upgrade --yes
RUN apt-get install --yes \
    build-essential \
    ca-certificates \
    curl \
    jq \
    squashfs-tools \
    --no-install-recommends \
    git \
    snapcraft \
    flatpak-builder \
    elfutils \
    --no-install-recommends
