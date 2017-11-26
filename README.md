# Geth-iOS
Home for pre-built Geth.framewok for iOS

## Notice

This repo holds pre-built, zipped copies of the [Geth](https://github.com/ethereum/go-ethereum) framework for the [iOS Kin SDK](https://github.com/kinfoundation/kin-sdk-core-ios)

It includes an i386 slice not currently available in the original Geth repo.

To build this library yourself from the Kin Foundation fork of Go-Ethereum:

```bash
$ git clone git@github.com:kinfoundation/go-ethereum.git
$ cd go-ethereum
$ git checkout make_ios_386
$ make ios
```

