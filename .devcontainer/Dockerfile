FROM mcr.microsoft.com/devcontainers/cpp:1-ubuntu-20.04

ARG REINSTALL_CMAKE_VERSION_FROM_SOURCE="3.22.2"

# Optionally install the cmake for vcpkg
COPY ./reinstall-cmake.sh /tmp/

RUN if [ "${REINSTALL_CMAKE_VERSION_FROM_SOURCE}" != "none" ]; then \
        chmod +x /tmp/reinstall-cmake.sh && /tmp/reinstall-cmake.sh ${REINSTALL_CMAKE_VERSION_FROM_SOURCE}; \
    fi \
    && rm -f /tmp/reinstall-cmake.sh

# set up display
RUN export DISPLAY=localhost:10.0

# install dependencies
RUN export DEBIAN_FRONTEND=noninteractive
RUN apt-get -y update
RUN apt-get -y upgrade
RUN apt-get -y install --no-install-recommends \
                libfreetype6-dev \
                libsfml-dev \
                libxrandr-dev \
                libxcursor-dev \
                libudev-dev \
                libopenal-dev \
                libfreetype-dev \
                libflac-dev \
                libvorbis-dev \
                libopenal-dev \
                libgl1-mesa-dev \
                libegl1-mesa-dev \
                libdrm-dev \
                libgbm-dev \
                libasound2-dev \
                libopencv-dev \
                xauth \
                x11-apps \
                x11-utils \
                tesseract-ocr \
                libtesseract-dev