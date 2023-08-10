Evadore uses the strong structure of the Ethereum network. Powered by Go-Ethereum.

Go Ethereum
Official Golang execution layer implementation of the Ethereum protocol.

Automated builds are available for stable releases and the unstable master branch. Binary archives are published at https://geth.ethereum.org/downloads/.

Building the source
For prerequisites and detailed build instructions please read the Installation Instructions.

Building geth requires both a Go (version 1.19 or later) and a C compiler. You can install them using your favourite package manager. Once the dependencies are installed, run

make geth
or, to build the full suite of utilities:

make all
