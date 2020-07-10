FROM rust

RUN apt-get update && apt-get install -y \
    docker.io

WORKDIR /home/rust/workdir
RUN rustup component add rust-analysis --toolchain 1.44.1-x86_64-unknown-linux-gnu
RUN rustup component add rls --toolchain 1.44.1-x86_64-unknown-linux-gnu
RUN cargo install cross

CMD sleep infinity