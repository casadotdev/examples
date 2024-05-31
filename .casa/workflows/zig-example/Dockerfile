FROM busybox AS base

# LABEL author="ziglings.org"
# LABEL description="Minimal docker container for using the Zig toolchain for automated testing."

ENV ZIG_VERSION=master
ENV ZIG_PATH=/zig/${ZIG_VERSION}/files

RUN wget -q https://github.com/marler8997/zigup/releases/download/v2024_03_13/zigup.ubuntu-latest-x86_64.zip && \
    unzip zigup.ubuntu-latest-x86_64.zip -d /usr/bin \
    && chmod +x /usr/bin/zigup \
    && zigup $ZIG_VERSION --install-dir /zig \
    && chmod -R a+w ${ZIG_PATH} \
    && rm zigup.ubuntu-latest-x86_64.zip /usr/bin/zigup

FROM busybox AS build

COPY --from=base /zig/master/files/lib /lib
COPY --from=base /usr/bin/zig /bin/zig

COPY /root/zig-example /root

CMD ["sh"]
