# AirPort configuration utility for Apple Airport Extreme etc.
#
# `./wine winecfg` to choose Windows 7 or newer.
# `./wine /usr/src/AirPortSetup.exe` to install.
# `./wine /wine/drive_c/Program\ Files/AirPort/APUtil.exe` to run.

FROM jess/wine

ENV WINEPREFIX=/wine WINEDLLOVERRIDES=mscoree=d

ADD \
  http://supportdownload.apple.com/download.info.apple.com/Apple_Support_Area/Apple_Software_Updates/Mac_OS_X/downloads/041-0257.20120611.MkI85/AirPortSetup.exe \
  /usr/src

COPY /entrypoint /
ENTRYPOINT ["/entrypoint"]
