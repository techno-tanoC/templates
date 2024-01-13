FROM rust:1.75.0-slim
WORKDIR /workspace

RUN <<EOF
  rustup component add rustfmt
  rustup component add clippy
  cargo install cargo-watch
EOF

RUN <<EOF
  apt update
  apt install -y make git wget
EOF
