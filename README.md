
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
