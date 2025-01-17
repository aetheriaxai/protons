# protons-benchmark <!-- omit in toc -->

[![ipfs.io](https://img.shields.io/badge/project-IPFS-blue.svg?style=flat-square)](http://ipfs.io)
[![IRC](https://img.shields.io/badge/freenode-%23ipfs-blue.svg?style=flat-square)](http://webchat.freenode.net/?channels=%23ipfs)
[![Discord](https://img.shields.io/discord/806902334369824788?style=flat-square)](https://discord.gg/ipfs)
[![codecov](https://img.shields.io/codecov/c/github/ipfs/protons.svg?style=flat-square)](https://codecov.io/gh/ipfs/protons)
[![CI](https://img.shields.io/github/workflow/status/ipfs/protons/test%20&%20maybe%20release/master?style=flat-square)](https://github.com/ipfs/protons/actions/workflows/js-test-and-release.yml)

> Protobuf to ts transpiler

## Table of contents <!-- omit in toc -->

- [Install](#install)
- [Usage](#usage)
- [License](#license)
- [Contribute](#contribute)

## Install

```console
$ npm i protons-benchmark
```

```console
$ git clone git@github.com:ipfs/protons.git
$ cd protons
$ npm i
$ cd packages/protons-benchmark
```

## Usage

Run the benchmark suite:

```console
$ npm start

> protons-benchmark@0.0.0 prestart
> npm run build


> protons-benchmark@0.0.0 build
> aegir build --no-bundle && cp -R src/protobufjs dist/src/protobufjs

[15:02:28] tsc [started]
[15:02:32] tsc [completed]

> protons-benchmark@0.0.0 start
> node dist/src/index.js

pbjs x 11,798 ops/sec ±4.58% (88 runs sampled)
protons x 11,693 ops/sec ±2.69% (85 runs sampled)
protobuf.js x 12,419 ops/sec ±1.66% (88 runs sampled)
@protobuf-ts x 10,536 ops/sec ±3.14% (85 runs sampled)
Fastest is protobuf.js
```

Or in a browser:

```console
$ npm run start:browser

> protons-benchmark@0.0.0 start:browser
> npx playwright-test dist/src/index.js --runner benchmark

✔ chromium set up
pbjs x 19,027 ops/sec ±0.86% (67 runs sampled)
protons x 18,901 ops/sec ±0.65% (67 runs sampled)
protobuf.js x 18,937 ops/sec ±0.55% (65 runs sampled)
@protobuf-ts x 16,669 ops/sec ±0.49% (68 runs sampled)
Fastest is pbjs,protobuf.js
```

## License

Licensed under either of

- Apache 2.0, ([LICENSE-APACHE](LICENSE-APACHE) / <http://www.apache.org/licenses/LICENSE-2.0>)
- MIT ([LICENSE-MIT](LICENSE-MIT) / <http://opensource.org/licenses/MIT>)

## Contribute

Feel free to join in. All welcome. Open an [issue](https://github.com/ipfs/js-ipfs-unixfs-importer/issues)!

This repository falls under the IPFS [Code of Conduct](https://github.com/ipfs/community/blob/master/code-of-conduct.md).

[![](https://cdn.rawgit.com/jbenet/contribute-ipfs-gif/master/img/contribute.gif)](https://github.com/ipfs/community/blob/master/CONTRIBUTING.md)
