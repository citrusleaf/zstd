FROM circleci/buildpack-deps:bionic@sha256:5ecd6d9cb3e0a74a2563a48baee224b6d79341638dc843d9072b4f08cf23be43

RUN sudo dpkg --add-architecture i386
RUN sudo apt-get -y -qq update
RUN sudo apt-get -y install \
    gcc-multilib-powerpc-linux-gnu gcc-arm-linux-gnueabi \
    libc6-dev-armel-cross gcc-aarch64-linux-gnu libc6-dev-arm64-cross \
    libc6-dev-ppc64-powerpc-cross zstd gzip coreutils \
    libcurl4-openssl-dev
