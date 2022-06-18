# Tutorial-Tauri

---

## Prerequisites

### Rust

#### Windows

* [Node.js](https://nodejs.org/ja/download/)
* `npm install -g yarn`

* [Build Tools for Visual Studio 2022](https://visualstudio.microsoft.com/visual-cpp-build-tools/)
  * C++ build tools
  * Windows 10 SDK

* [WebView2](https://developer.microsoft.com/en-us/microsoft-edge/webview2/#download-section) (Windows 11ではプリインストールされている)

* [rustup](https://www.rust-lang.org/tools/install)
  * [DOWNLOAD RUSTUP-INIT.EXE (64-BIT)](https://static.rust-lang.org/rustup/dist/x86_64-pc-windows-msvc/rustup-init.exe)

#### Mac

```bash
brew install node
npm install -g yarn

xcode-select --install

curl --proto '=https' --tlsv1.2 https://sh.rustup.rs -sSf | sh
```

#### Confirmation and update

```bash
node -v

rustc --version
cargo --version

rustup update

```

### Tauri

```bash
cargo install tauri-cli --version "^1.0.0"

cargo tauri --help
```

## Create app

```bash
npx create-tauri-app

? What is your app name? (tauri-app)
# my-tauri-app

? What should the window title be? (Tauri App)
# My Tauri App

? What UI recipe would you like to add? (Use arrow keys)
> Vanilla.js (html, css, and js without the bundlers)
  create-vite (vanilla, vue, react, svelte, preact, lit) (https://vitejs.dev/guide/#scaffolding-your-first-vite-project)
  create-react-app (https://create-react-app.dev/)
  Svelte (https://github.com/sveltejs/template)
  Solid (https://github.com/solidjs/templates)
  Vue CLI (https://cli.vuejs.org/)
  Angular CLI (https://angular.io/cli)
(Move up and down to reveal more choices)
# Vanilla.js (html, css, and js without the bundlers)
```

```bash
cd my-tauri-app
npm install
npm run tauri dev
```

## Build

```bash
npm run tauri build

ls ./src-tauri/target/release/my-tauri-app.exe
```

---

Copyright (c) 2022 YA-androidapp(https://github.com/YA-androidapp) All rights reserved.
