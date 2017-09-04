# NeoSwift
Swift Wrapper for Neo Blockchain API

Currently supporting
```
enum RPCMethod: String {
        case getBestBlockHash = "getbestblockhash"
        case getBlock = "getblock"
        case getBlockCount = "getblockcount"
        case getBlockHash = "getblockhash"
        case getConnectionCount = "getconnectioncount"
        case getTransaction = "getrawtransaction"
        case getTransactionOutput = "gettxout"
        case getUnconfirmedTransactions = "getrawmempool"
        case sendTransaction = "sendrawtransaction"
        //The following routes can't be invoked by calling an RPC server
        //We must use the wrapper for the nodes made by COZ
        case getBalance = "getbalance"
    }
```

Underlying crypto methods are using native golang compiled via gomobile.
[https://github.com/apisit/neo-wallet-address-go](https://github.com/apisit/neo-wallet-address-go)
[https://github.com/apisit/btckeygenie](https://github.com/apisit/btckeygenie)

Need to bring these under one umbrella
