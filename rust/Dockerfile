FROM rust

RUN apt-get update && apt-get install -y \
    docker.io

WORKDIR /home/rust/workdir

# recommend of rust extension
RUN rustup component add rust-analysis --toolchain 1.44.1-x86_64-unknown-linux-gnu
RUN rustup component add rls --toolchain 1.44.1-x86_64-unknown-linux-gnu

# setting for build Windows binary
RUN apt install -y mingw-w64
RUN rustup target add x86_64-pc-windows-gnu

CMD sleep infinity