# Geth-iOS
Home for pre-built Geth.framewok for iOS

## Notice

This repo holds pre-built, zipped copies of the [Geth](https://github.com/ethereum/go-ethereum) framework for the [iOS Kin SDK](https://github.com/kinfoundation/kin-sdk-core-ios)

It includes an i386 slice not currently available in the original Geth repo.

To build this library yourself from the Kin Foundation fork of Go-Ethereum:

```bash
$ git clone git@github.com:kinfoundation/kinfoundation/kin-sdk-core-ios.git
$ cd go-ethereum
$ git checkout master
$ git pull
$ git checkout make_ios_386
$ git pull --rebase master
$ make ios
$ open build/bin
```
right click on Geth.framework choose compress.

```bash
$ git clone --depth=1 git@github.com:kinfoundation/Geth-iOS.git 
$ open Geth-iOS
```

Drag Geth-framework.zip into Geth-iOS

```bash
$ cd Geth-iOS
$ git add .
$ git commit -m "updated framework"
$ git push
```
This will place latest Geth-framework buyild into Geth-iOS.
The pod spec in kinfoundation/kin-sdk-core-ios uses the HEAD of master
The only other thing to do is to bump the pod spec to make sure host app will fetch latest change

