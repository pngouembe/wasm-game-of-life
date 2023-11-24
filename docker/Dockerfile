FROM rust:1.69

RUN apt update && apt install -y \
  nodejs \
  npm

RUN cargo install wasm-pack
RUN cargo install wasm-bindgen-cli
RUN rustup target add wasm32-unknown-unknown

RUN npm install -g n
RUN n 12.22.12
