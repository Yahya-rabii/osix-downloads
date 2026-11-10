# Third-party software in the Osix apps

The Osix apps (Android, Windows, macOS, Linux) are built from the same code as
[devtools.osixlab.com](https://devtools.osixlab.com). They include the open-source
components below. Each keeps its own licence; the Osix code itself is
© OsixLab, all rights reserved.

## Copyleft components, and where their source is

| Component | Licence | Used for | Source |
|---|---|---|---|
| FFmpeg, as the ffmpeg.wasm core 0.12.10 (built with x264, x265 and other GPL libraries) | GPL-2.0-or-later | Video and GIF tools on the device | https://github.com/ffmpegwasm/ffmpeg.wasm (tag `v0.12.10`), https://ffmpeg.org |
| Stockfish (stockfish.js, single-threaded lite build) | GPL-3.0 | Chess opponent | https://github.com/nmrugg/stockfish.js, https://github.com/official-stockfish/Stockfish |
| LibreSpeed (`speedtest.js`, `speedtest_worker.js`) | LGPL-3.0-or-later | Speed test | https://github.com/librespeed/speedtest. Our copy changes only the worker path and ships as readable source inside the app. |

These run as separate WebAssembly or JavaScript workers and are not linked into
the rest of Osix. If you need the exact corresponding source for a release and
cannot get it from the links above, open an issue in this repository.

## Bundled applications

| Application | Licence | Copyright |
|---|---|---|
| draw.io (diagram editor) | Apache-2.0 | JGraph Ltd |
| CyberChef (data toolkit) | Apache-2.0 | Crown Copyright (GCHQ) |
| miniPaint (image editor) | MIT | ViliusL |
| Excalidraw (whiteboard) | MIT | Excalidraw |
| Mermaid (diagrams) | MIT | Knut Sveidqvist |
| Tesseract OCR engine and the 15 `tessdata_best` language models | Apache-2.0 | Google, tesseract-ocr contributors |
| Liberation Sans font | SIL Open Font License 1.1 | Red Hat, Inc. |

## App shells

| Component | Licence | Notes |
|---|---|---|
| Electron (desktop apps) | MIT | Chromium's and Node.js's own notices are inside each desktop build (`LICENSES.chromium.html`, `LICENSE`). |
| Capacitor (Android app) | MIT | Drifty Co. |

## Downloaded at your request, not bundled

- **Qwen3** language models for the AI Assistant: Apache-2.0, Alibaba Cloud (Qwen team).
- **Opus-MT** translation models: CC-BY-4.0. J. Tiedemann and S. Thottingal, "OPUS-MT — Building open translation services for the World", EAMT 2020.
- **Whisper** speech model: MIT, OpenAI.
- **Kiwix `.zim` books** (Wikipedia, WikiMed, …) each carry their own content licence, mostly CC BY-SA. Osix's ZIM reader is its own code, written from the openZIM specification; no libzim code is included.

## Direct dependencies

Every npm package the apps depend on directly, with the licence it declares.
Their own dependencies are bundled too, under the licences they declare.

| Package | Version | Licence |
|---|---|---|
| ajv | 8.18.0 | MIT |
| ajv-formats | 3.0.1 | MIT |
| axios | 1.13.6 | MIT |
| bcryptjs | 3.0.3 | BSD-3-Clause |
| bwip-js | 4.11.2 | MIT |
| canvas-confetti | 1.9.4 | ISC |
| @capacitor/android | 7.6.10 | MIT |
| @capacitor/app | 7.1.2 | MIT |
| @capacitor/core | 7.6.10 | MIT |
| chess.js | 1.4.0 | BSD-2-Clause |
| class-variance-authority | 0.7.1 | Apache-2.0 |
| clsx | 2.1.1 | MIT |
| cronstrue | 3.24.0 | MIT |
| cubejs | 1.3.2 | MIT |
| diff | 8.0.3 | BSD-3-Clause |
| @duckdb/duckdb-wasm | 1.33.1-dev57.0 | MIT |
| @excalidraw/excalidraw | 0.18.1 | MIT |
| exifr | 7.1.3 | MIT |
| @faker-js/faker | 10.3.0 | MIT |
| fast-xml-parser | 5.4.1 | MIT |
| @ffmpeg/core | 0.12.10 | GPL-2.0-or-later |
| @ffmpeg/ffmpeg | 0.12.15 | MIT |
| @ffmpeg/util | 0.12.2 | MIT |
| figlet | 1.11.4 | MIT |
| @finos/perspective | 3.8.0 | Apache-2.0 |
| @finos/perspective-viewer | 3.8.0 | Apache-2.0 |
| @finos/perspective-viewer-d3fc | 3.8.0 | Apache-2.0 |
| @finos/perspective-viewer-datagrid | 3.8.0 | Apache-2.0 |
| framer-motion | 12.34.3 | MIT |
| fzstd | 0.1.1 | MIT |
| gpt-tokenizer | 3.4.0 | MIT |
| grapesjs | 0.23.4 | BSD-3-Clause |
| graphql | 16.14.2 | MIT |
| hash-wasm | 4.12.0 | MIT |
| html-to-image | 1.11.13 | MIT |
| @huggingface/transformers | 4.2.0 | Apache-2.0 |
| jmespath | 0.16.0 | Apache-2.0 |
| jose | 6.1.3 | MIT |
| js-chess-engine | 1.0.3 | MIT |
| js-yaml | 4.1.1 | MIT |
| jsonpath-plus | 10.4.0 | MIT |
| jszip | 3.10.1 | (MIT OR GPL-3.0-or-later) |
| libphonenumber-js | 1.13.9 | MIT |
| lucide-react | 0.575.0 | ISC |
| mammoth | 1.13.0 | BSD-2-Clause |
| @marp-team/marp-core | 4.4.0 | MIT |
| mermaid | 11.16.0 | MIT |
| monaco-editor | 0.56.0 | MIT |
| @monaco-editor/react | 4.7.0 | MIT |
| next-themes | 0.4.6 | MIT |
| @noble/curves | 2.2.0 | MIT |
| @noble/hashes | 2.2.0 | MIT |
| opentype.js | 2.0.0 | MIT |
| pako | 3.0.1 | (MIT AND Zlib) |
| pdf-lib | 1.17.1 | MIT |
| @pdf-lib/fontkit | 1.1.1 | MIT |
| pdfjs-dist | 6.2.108 | Apache-2.0 |
| @pdfme/common | 6.1.12 | MIT |
| @pdfme/generator | 6.1.12 | MIT |
| @pdfme/schemas | 6.1.12 | MIT |
| @pdfme/ui | 6.1.12 | MIT |
| peerjs | 1.5.5 | MIT |
| pixelmatch | 7.2.0 | ISC |
| prettier | 3.9.6 | MIT |
| qrcode | 1.5.4 | MIT |
| radix-ui | 1.4.3 | MIT |
| react | 19.2.4 | MIT |
| react-dom | 19.2.4 | MIT |
| react-dropzone | 15.0.0 | MIT |
| react-image-crop | 11.0.10 | ISC |
| react-markdown | 10.1.0 | MIT |
| react-router-dom | 7.13.1 | MIT |
| @react-three/drei | 10.7.8 | MIT |
| @react-three/fiber | 9.7.0 | MIT |
| remark-gfm | 4.0.1 | MIT |
| rxjs | 7.8.2 | Apache-2.0 |
| semver | 7.8.5 | ISC |
| simple-icons | 16.28.0 | CC0-1.0 |
| smol-toml | 1.7.1 | BSD-3-Clause |
| sonner | 2.0.7 | MIT |
| sql-formatter | 15.7.2 | MIT |
| sql.js | 1.14.1 | MIT |
| stockfish | 18.0.8 | GPL-3.0 |
| sudoku-core | 3.0.3 | MIT |
| swagger-ui-dist | 5.32.0 | Apache-2.0 |
| swagger-ui-react | 5.32.0 | Apache-2.0 |
| tailwind-merge | 3.5.0 | MIT |
| tailwindcss | 4.2.1 | MIT |
| @tailwindcss/typography | 0.5.19 | MIT |
| @tailwindcss/vite | 4.2.1 | MIT |
| @tanstack/react-query | 5.90.21 | MIT |
| tesseract.js | 7.0.0 | Apache-2.0 |
| @tesseract.js-data/eng | 1.0.0 | MIT |
| three | 0.185.1 | MIT |
| turndown | 7.2.4 | MIT |
| @types/canvas-confetti | 1.9.0 | MIT |
| @types/jmespath | 0.15.2 | MIT |
| @types/sql.js | 1.4.11 | MIT |
| @types/three | 0.185.4 | MIT |
| @uiw/react-json-view | 2.0.0-alpha.41 | MIT |
| @univerjs/presets | 0.25.1 | Apache-2.0 |
| xlsx | 0.18.5 | Apache-2.0 |
| @xyflow/react | 12.11.2 | MIT |
| zustand | 5.0.11 | MIT |
| @zxing/browser | 0.2.1 | MIT |
