FROM buildpack-deps:jessie-curl

LABEL maintainer "mattias@ppelgren.se"

ARG PKGDIFF_VERSION=1.7.2

RUN apt-get update && apt-get install -y \
    perl \
    make \
    wdiff \
    file \
 && rm -rf /var/lib/apt/lists/*

RUN curl -sSL https://github.com/lvc/pkgdiff/archive/${PKGDIFF_VERSION}.tar.gz \
    | tar -xz \
    && cd pkgdiff-${PKGDIFF_VERSION} \
    && make install prefix=/usr \
    && cd .. \
    && rm -r pkgdiff-${PKGDIFF_VERSION}

ENTRYPOINT ["pkgdiff"]
