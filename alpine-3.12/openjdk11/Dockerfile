FROM blankhang/alpine-3.12:glibc-2.32-r0
MAINTAINER blankhang <blankhang@gmail.com>
RUN apk add --no-cache openjdk11 && \
    ln -s /usr/lib/libfontconfig.so.1 /usr/lib/libfontconfig.so && \
    ln -s /lib/libuuid.so.1 /usr/lib/libuuid.so.1 && \
    ln -s /lib/libc.musl-x86_64.so.1 /usr/lib/libc.musl-x86_64.so.1
ENV LD_LIBRARY_PATH /usr/lib