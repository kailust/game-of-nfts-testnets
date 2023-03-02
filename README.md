# game-of-nfts-testnets

Follow this
```
https://github.com/game-of-nfts/gon-testnets/blob/main/doc/instruction-erc721.md#transaction
```

## Task 1
```
A1	1	Create one Collection on IRISnet	Must set ClassUri and ClassData	TxHash on IRISnet
```
 Use IRIS GO SDK
 ```
 https://www.irisnet.org/docs/get-started/install.html#install-go
 ```
 Testnet endpoints
 ```
GRPC: 35.234.10.84:9090
RPC: http://35.234.10.84:26657/
REST: http://35.234.10.84:1317/swagger/
```
First add key
```
iris keys add Mykey --recover
```
Using CLI
```
iris tx nft issue "myNFR" --from="Mykey" --name="MyNFT" --symbol="MYNFT" --mint-restricted=false --update-restricted=false  --chain-id=nyancat-8 --node=http://35.234.10.84:26657/
```