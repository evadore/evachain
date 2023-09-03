### For example startnode.sh
geth --datadir /home/cdata --networkid 32611 --snapshot=false --port 30303 --ipcdisable --bootnodes enode://31c06baafa46158aadc036dc76824f15607fdbd5c49afe292071b782bd7ceeda18f3a1167eab42bbf72a512a99bb08fc97df4664aa32262ee6fcc1464fba5856@89.252.140.146:29061,enode://31c06baafa46158aadc036dc76824f15607fdbd5c49afe292071b782bd7ceeda18f3a1167eab42bbf72a512a99bb08fc97df4664aa32262ee6fcc1464fba5856@188.132.176.178:29061 --syncmode full --gcmode full

### If you want to become a block signer, you must do these steps.

1 -) geth --init <datadir> account new

2 - ) Create /home/cdata/password.txt and into your wallet password.

3 - ) You must send us the wallet address you created to submit it for authorization confirmation on our network.

4 - ) geth --datadir /home/cdata --networkid 32611 --snapshot=false --port 30303 --ipcdisable --http --http.addr 0.0.0.0 --http.corsdomain '*' --http.api admin,debug,web3,eth,txpool,personal,clique,miner,net --ws --ws.addr 0.0.0.0 --ws.origins '*' --ws.api admin,debug,web3,eth,txpool,personal,clique,miner,net --http.port=80 --http.vhosts='*' --bootnodes enode://31c06baafa46158aadc036dc76824f15607fdbd5c49afe292071b782bd7ceeda18f3a1167eab42bbf72a512a99bb08fc97df4664aa32262ee6fcc1464fba5856@89.252.140.146:29061,enode://31c06baafa46158aadc036dc76824f15607fdbd5c49afe292071b782bd7ceeda18f3a1167eab42bbf72a512a99bb08fc97df4664aa32262ee6fcc1464fba5856@188.132.176.178:29061 --allow-insecure-unlock --unlock <wallet addr> --password /home/cdata/password.txt --miner.etherbase <wallet addr> --mine --syncmode full --gcmode full
