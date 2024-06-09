# Yew Tutorial Project

This project is a basic tutorial for Yew, a framework for building interactive web applications with Rust.

## Requirements

- [Rust](https://www.rust-lang.org/tools/install)
- [Trunk](https://trunkrs.dev/#install)
- [wasm-bindgen-cli](https://rustwasm.github.io/wasm-bindgen/)

## Installation

First, make sure you have Rust installed. Then, install Trunk and wasm-bindgen-cli:

```sh
cargo install trunk
rustup target add wasm32-unknown-unknown
```

## Project Structure

```plaintext
src/
├── components/
│   ├── mod.rs
│   ├── video_details.rs
|   ├── videos_list.rs
│   └── app.rs
├── main.rs
├── models/
│   ├── mod.rs
│   └── video.rs
├── mod.rs
static/
│   └── index.html
Cargo.toml
```

## Running the Project
To run the project, use the following command:

```sh
trunk serve --proxy-backend=https://yew.rs/tutorial
```

This command will start a development server and serve your application at http://localhost:8080. The --proxy-backend parameter is used to proxy requests to https://yew.rs/tutorial.