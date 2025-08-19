## Project Introduction

[Ton browser] is a truly independent web browser, using a novel engine based on web standards.

> [!IMPORTANT]
> Ton browser is in a pre-alpha state, and only suitable for use by developers
>

## Developer Information

Developer：Diego Gletton Nunes
Develop Date：2025年6月29日


## Features

We aim to build a complete, usable browser for the modern web.

Ton browser uses a multi-process architecture with a main UI process, several WebContent renderer processes,
an ImageDecoder process, and a RequestServer process.

Image decoding and network connections are done out of process to be more robust against malicious content.
Each tab has its own renderer process, which is sandboxed from the rest of the system.

At the moment, many core library support components are inherited from SerenityOS:

- LibWeb: Web rendering engine
- LibJS: JavaScript engine
- LibWasm: WebAssembly implementation
- LibCrypto/LibTLS: Cryptography primitives and Transport Layer Security
- LibHTTP: HTTP/1.1 client
- LibGfx: 2D Graphics Library, Image Decoding and Rendering
- LibUnicode: Unicode and locale support
- LibMedia: Audio and video playback
- LibCore: Event loop, OS abstraction layer
- LibIPC: Inter-process communication

## How do I build and run this?

See for information on how to build Ton browser.

Ton browser runs on Linux, macOS, Windows (with WSL2), and many other \*Nixes.

## How do I read the documentation?

Code-related documentation can be found in the folder.

## Get in touch and participate!

Join to participate in development discussion.

Please read  if you plan to contribute for the first time.

Before opening an issue, please see the (ISSUES.md).

The full contribution guidelines can be found in (CONTRIBUTING.md).

## License

Ton browser is licensed under a 2-clause BSD license.
