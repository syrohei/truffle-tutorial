# truffle-tutorial

## getting satared

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


## test
```
truffle test


