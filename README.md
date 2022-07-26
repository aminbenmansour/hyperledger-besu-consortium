# hyperledger-besu-private-network

IBFT, a proof-of-authority algorithm, requires a minimum of 4 nodes to operate, one of them will be bootnode and others will be validators.


nodes doesn’t have any idea about the other nodes, the centralized blockchain has the main bootnode that connects the nodes. So what we have to do is to start the bootnode and copy its enode url and provide it in the other nodes config file. The propery in the toml config file is `bootnodes`.
