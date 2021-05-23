# README

## Repository Tools

### [Developer tools](devtools.md) \#\#\#

Specific tools for developers working on this repository. Contains the script `github-merge.py` for merging GitHub pull requests securely and signing them using GPG.

### [Verify-Commits](verify-commits.md) \#\#\#

Tool to verify that every merge commit was signed by a developer using the above `github-merge.py` script.

### [Linearize](linearize.md) \#\#\#

Construct a linear, no-fork, best version of the blockchain.

### [Qos](qos.md) \#\#\#

A Linux bash script that will set up traffic control \(tc\) to limit the outgoing bandwidth for connections to the Dogecoin network. This means one can have an always-on dogecoind instance running, and another local dogecoind/dogecoin-qt instance which connects to this node and receives blocks from it.

### [Seeds](seeds.md) \#\#\#

Utility to generate the pnSeed\[\] array that is compiled into the client.

## Build Tools and Keys

### [Debian](debian.md) \#\#\#

Contains files used to package dogecoind/dogecoin-qt for Debian-based Linux systems. If you compile dogecoind/dogecoin-qt yourself, there are some useful files here.

### [Gitian-descriptors](gitian-descriptors.md) \#\#\#

Notes on getting Gitian builds up and running using KVM.

### [Gitian-keys](gitian-keys.md)

PGP keys used for signing Dogecoin Core [Gitian release](../doc/release-process.md) results.

### [MacDeploy](macdeploy.md) \#\#\#

Scripts and notes for Mac builds.

### [RPM](rpm.md) \#\#\#

RPM spec file for building dogecoin-core on RPM based distributions

### [Gitian-build](https://github.com/TelsaCoin/TelsaCoin/tree/db7abb962b5bfc7a23084bed38eeebc9083eb1b2/contrib/gitian-build.sh) \#\#\#

Script for running full Gitian builds.

## Test and Verify Tools

### [TestGen](testgen.md) \#\#\#

Utilities to generate test vectors for the data-driven Dogecoin tests.

### [Verify Binaries](verifybinaries.md) \#\#\#

This script attempts to download and verify the signature file SHA256SUMS.asc from dogecoin.com.

