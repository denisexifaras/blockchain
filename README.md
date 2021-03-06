
Assume golang installed

```
$cd ~
$mkdir BlockchainSetup
$cd BlockchianSetup
$ mkdir GOCODE
$ cd GOCODE
$ mkdir src
$ mkdir pkg
$ mkdir bin
$ cd src
$ go get <github repo with go>
$ cd githbu.com....
$ make
$ mkdir hyperledger
$ cd hyperledger
$ git clone git@github.com:hyperledger/fabric.git
$ cd fabric
$ git fetch
$ git checkout v0.6
```

Install docker from: https://docs.docker.com/engine/getstarted/step_one/#/step-2-install-docker

```
$ docker pull hyperledger/fabric-peer:latest
$ docker pull hyperledger/fabric-membersrvc:latest
```

We clean up IBM code from <a href="https://github.com/IBM-Blockchain/marbles/blob/master/chaincode/marbles_chaincode.go" target="_blank">here</a>, to create `templatego.md`. This has the minimum number of functions required to start interacting with the blockchain. If the file is renamed to `template.go` it should build.

Make sure `github.com/hyperledger/fabric` is in branch `v0.6`.
From `github.com/*/blockchain` type `go build .` and this should return errors about importing unnecessary libraries. 

Edit `main.go` to interact with the blockchain. Start the docker container from `blockchain-docker-compose/one-peer-one-ca` using `docker-compose up` (or `docker-compose start` if already initialised once).
