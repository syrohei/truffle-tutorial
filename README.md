# truffle-tutorial

## getting started

```
npm install -g truffle
```
private-chain

```
geth --datadir ./private init ./genesis.json
```
```
geth --datadir ./private account new
```
```
geth --datadir ./private --networkid 123456 --nodiscover --maxpeers 0 --rpc --rpcapi eth,net,web3,personal,admin,miner --minerthreads 1 --rpccorsdomain "*" --mine
```

```
>personal.newAccount()
>eth.sendTransaction({from: eth.coinbase, to: personal.listAccounts[1] , value: web3.toWei(1, "ether")})
```

public-chain

```
geth --datadir ./main account new
```

geth をmain-netで起動（eth)

```
$ geth --datadir ./main --rpc --rpcaddr "0.0.0.0" --rpcapi eth,net,web3,personal,admin,miner --rpccorsdomain "*" --support-dao-fork
```
geth をmain-netで起動（etc)

```
$ geth --datadir ./main --rpc --rpcaddr "0.0.0.0" --rpcapi eth,net,web3,personal,admin,miner --rpccorsdomain "*" --oppose-dao-fork
```

```
$ truffle migrate
```
```
$ truffle build
```

## develop
```
$ truffle serve
```

## test
```
$ truffle test
```

### donate
```
bitcoin : 1257U991WqSvhpS65NjMEoWH5UBwQH5N3V 

eth :0xbf2b26c21c6a1b248d9c857be756fa3bf261aff1

etc :0xbf91930d9a12c365385f310792951d792115d095
```
