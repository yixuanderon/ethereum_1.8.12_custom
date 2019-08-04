# go-ethereum

this repository makes some changes to go-ethereum(v1.8.12) for the purpose of custom ethereum development 

- the difficulty of ethash algorithm is always equal to 1.
- 1block / 1s when pending txpool is not empty, 1block/ 5s when pending txpool is empty.
- the constant——GenesisGasLimit is increased to 1463219498106.
- the constant——FrontierBlockReward is increased to big.NewInt(9e+18).
- the constant——TxGas is decreased to 0 from 21000.
- the default value of Gas is decreased to 0 from 90000.
- all variables of DefaultTxPoolConfig are increased to 99999999.
- add two new json-rpc methods——eth_getSentTransactionsList and eth_getConfirmedTransactionsList.