FROM debian

RUN \
  apt-get update && \
  apt-get -y install \
    curl \
    openjdk-7-jre \
    xz-utils \
    && \
  apt-get clean

RUN curl -sS https://downloads.arduino.cc/arduino-1.6.7-linux64.tar.xz | tar xJ

WORKDIR /arduino-1.6.7
CMD ["/arduino-1.6.7/arduino"]
