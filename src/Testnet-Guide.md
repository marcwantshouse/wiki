# Testnet Guide

The installation of full node for testnet is the same as the mainnet: [Full Node Starter Guide](Full-Node-Starter-Guide.md) 

**The user.conf must be modified before starting the full node**

Please note that the default address and port for the REST API is http://127.0.0.1:12973/docs.

## Configuration

In the `$HOME/alephium/user.conf` (`user-mainnet.conf` if docker is used) file you have to add:
```
alephium.network.network-id = 1
alephium.discovery.bootstrap = ["testnet-bootstrap0.alephium.org:9973","testnet-bootstrap1.alephium.org:9973"]

```

## Mining
In the testnet you can use the [CPU Miner Guide](CPU-Miner-Guide.md) to get some ALPH

Append your miner addresses in `$HOME/alephium/user.conf` like:

```
alephium.mining.miner-addresses = [ 
"1FsroWmeJPBhcPiUr37pWXdojRBe6jdey9uukEXk1TheA",
"1CQvSXsmM5BMFKguKDPpNUfw1idiut8UifLtT8748JdHc",
"193maApeJWrz9GFwWCfa982ccLARVE9Y1WgKSJaUs7UAx",
"16fZKYPCZJv2TP3FArA9FLUQceTS9U8xVnSjxFG9MBKyY"
]
```

## Configuration example

```
alephium.network.network-id = 1
alephium.discovery.bootstrap = ["testnet-bootstrap0.alephium.org:9973","testnet-bootstrap1.alephium.org:9973"]
alephium.mining.miner-addresses = [ 
"1FsroWmeJPBhcPiUr37pWXdojRBe6jdey9uukEXk1TheA",
"1CQvSXsmM5BMFKguKDPpNUfw1idiut8UifLtT8748JdHc",
"193maApeJWrz9GFwWCfa982ccLARVE9Y1WgKSJaUs7UAx",
"16fZKYPCZJv2TP3FArA9FLUQceTS9U8xVnSjxFG9MBKyY"
]

```
