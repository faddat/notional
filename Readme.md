# Notional
Notional provides services in blockchain technology, including:

* Validation
* Relaying
* Software Development
   * Dig
   * Anone
   * CraftEconomy 
* Consulting and strategy

## Validation
Notional is an **active set** validator on:
1) [Osmosis](https://www.mintscan.io/osmosis/validators/osmovaloper1083svrca4t350mphfv9x45wq9asrs60c6rv0j5)
2) [Starname](https://www.mintscan.io/starname/validators/starvaloper1pdqlmncych8uzsfdnsptv7s0wpazc0rgv7zc6h)
3) [Regen](https://regen.aneka.io/validators/regenvaloper1083svrca4t350mphfv9x45wq9asrs60ct2p9a5)
4) [Akash](https://www.mintscan.io/akash/validators/akashvaloper1083svrca4t350mphfv9x45wq9asrs60c0k5a63)
5) [Gaia](https://www.mintscan.io/cosmos/validators/cosmosvaloper1083svrca4t350mphfv9x45wq9asrs60cdmrflj)
6) [Sentinel](https://www.mintscan.io/sentinel/validators/sentvaloper1083svrca4t350mphfv9x45wq9asrs60cv37gc8)
7) [E-Money](https://emoney.bigdipper.live/validators/emoneyvaloper16dc379m0qj64g4pr4nkl7ewak52qy2srpe6lxp)
8) [Ixo](https://blockscan.ixo.world/validator/ixovaloper1083svrca4t350mphfv9x45wq9asrs60camel0h)
9) [Juno](https://juno.aneka.io/validators/junovaloper1083svrca4t350mphfv9x45wq9asrs60cpqzg0y)
10) [Sifchain](https://www.mintscan.io/sifchain/validators/sifvaloper1083svrca4t350mphfv9x45wq9asrs60cyssqu6)


Notional is validating, but not in the active set:
* Umee

Notional wishes to validate:
* Every IBC-enabled blockchain


Notional has decided to maintain relayers for all chains -- and [document processes](./relaying-guide) -- on all chains where we are in the active validator set.  Presently, that means that we will maintain relayers on 50 channels.  If you are a community member or team that wants to see notional relay for your community, please put an issue on this repository and we will set up a relayer.  

## Comission
Notional charges a commission of 9.69% across all blockchains.


## Archive Nodes
Notional maintains archive nodes for BSC, Ethereum, Bitcoin, and every IBC-enabled Cosmos-SDK blockchain.  Documentation is kept in node-setup/archive and takes the approach that archive nodes are best setup slowly, even if that takes days or requires swapping out the binary during sync.  They're intended to be full, proper archives.  Time and expense are not spared in getting them into operation.  We run our archive nodes in three places:

* Hetzner.de (rented hardware)
* Notional HQ (own hardware)

Our archive nodes feed into our IPFS snapshot distribution system.


## Relaying

Notional Operates an omni-network [Go Relayer] On-Premesis in Hanoi.  Addresses are:

| Network      | Current Relayer Address | Former Relayer Address
| ----------- | ----------- | ------------ | 
| Regen      | regen1yeac5tgm4mqwl4fyrqp34s0gq5fy8ugx8s4x6u | regen1083svrca4t350mphfv9x45wq9asrs60chduq99|
| Osmosis   | osmo1yeac5tgm4mqwl4fyrqp34s0gq5fy8ugxsfd262   | osmo1083svrca4t350mphfv9x45wq9asrs60cq5yv9n |
| Gaia      | cosmos1yeac5tgm4mqwl4fyrqp34s0gq5fy8ugxcj76vc | cosmos1083svrca4t350mphfv9x45wq9asrs60cg0hunp |
| Akash     | akash1yeac5tgm4mqwl4fyrqp34s0gq5fy8ugx4fna4z  | akash1083svrca4t350mphfv9x45wq9asrs60c956m2m |
| Sentinel  | sent1yeac5tgm4mqwl4fyrqp34s0gq5fy8ugxrfgrgh   | sent1083svrca4t350mphfv9x45wq9asrs60cn5p9hw      |
| Sifchain   | sif1yeac5tgm4mqwl4fyrqp34s0gq5fy8ugxa03vrn   | sif1083svrca4t350mphfv9x45wq9asrs60cdjc2u2  |
| Starname   | star1t090jl87cnu9p3nlc6n20falgal2m8lujafd6u  | star1pdqlmncych8uzsfdnsptv7s0wpazc0rgf4xgk7 |
| Iris       | iaa1yeac5tgm4mqwl4fyrqp34s0gq5fy8ugxds7twf   | iaa1083svrca4t350mphfv9x45wq9asrs60cadhd3s  |
| Crypto.org | cro1qxd33n5ncsx4rdalmgy7hfufqpfcwysudqntax   | cro1mjdxgm2ndu9a4zmr9t3kq88fww30ms7q60e03h  |
| Persistence| persistence1xht3mqp946k7vm2j50yxywfg86pauhm9c2tmgt | persistence1r50r8cx09ege6206k70509a3cgk7npn3plg7r8 |




Notional Operates an IBC Relayer using [Hermes](https://github.com/informalsystems/ibc-rs) on the following networks, using the following addresses:


| Network      | Current Relayer Address | Former Relayer Address
| ----------- | ----------- | ------------ | 
| Regen      | regen1yeac5tgm4mqwl4fyrqp34s0gq5fy8ugx8s4x6u | regen1083svrca4t350mphfv9x45wq9asrs60chduq99|
| Osmosis   | osmo1yeac5tgm4mqwl4fyrqp34s0gq5fy8ugxsfd262   | osmo1083svrca4t350mphfv9x45wq9asrs60cq5yv9n |
| Gaia      | cosmos1yeac5tgm4mqwl4fyrqp34s0gq5fy8ugxcj76vc | cosmos1083svrca4t350mphfv9x45wq9asrs60cg0hunp |
| Akash     | akash1yeac5tgm4mqwl4fyrqp34s0gq5fy8ugx4fna4z  | akash1083svrca4t350mphfv9x45wq9asrs60c956m2m |
| Sentinel  | sent1yeac5tgm4mqwl4fyrqp34s0gq5fy8ugxrfgrgh   | sent1083svrca4t350mphfv9x45wq9asrs60cn5p9hw      |
| Sifchain   | sif1yeac5tgm4mqwl4fyrqp34s0gq5fy8ugxa03vrn   | sif1083svrca4t350mphfv9x45wq9asrs60cdjc2u2  |
| Starname   | star1t090jl87cnu9p3nlc6n20falgal2m8lujafd6u  | star1pdqlmncych8uzsfdnsptv7s0wpazc0rgf4xgk7 |
| Iris       | iaa1yeac5tgm4mqwl4fyrqp34s0gq5fy8ugxds7twf   | iaa1083svrca4t350mphfv9x45wq9asrs60cadhd3s  |
| Crypto.org | cro1qxd33n5ncsx4rdalmgy7hfufqpfcwysudqntax   | cro1mjdxgm2ndu9a4zmr9t3kq88fww30ms7q60e03h  |
| Persistence| persistence1xht3mqp946k7vm2j50yxywfg86pauhm9c2tmgt | persistence1r50r8cx09ege6206k70509a3cgk7npn3plg7r8 |



Notional has retired some relayer addresses:

| Network      |  Retired Relayer Address                         |
| ----------- | -----------                                       |
| Regen      | regen1083svrca4t350mphfv9x45wq9asrs60chduq99       |
| Osmosis   |  osmo1083svrca4t350mphfv9x45wq9asrs60cq5yv9n        |
| Gaia      | cosmos1083svrca4t350mphfv9x45wq9asrs60cg0hunp       |
| Akash     | akash1083svrca4t350mphfv9x45wq9asrs60c956m2m        |
| Sentinel  | sent1083svrca4t350mphfv9x45wq9asrs60cn5p9hw         |
| Sifchain   | sif1083svrca4t350mphfv9x45wq9asrs60cdjc2u2         |
| Starname   | star1pdqlmncych8uzsfdnsptv7s0wpazc0rgf4xgk7        |
| Iris       | iaa1083svrca4t350mphfv9x45wq9asrs60cadhd3s         |
| Crypto.org | cro1mjdxgm2ndu9a4zmr9t3kq88fww30ms7q60e03h         |
| Persistence| persistence1r50r8cx09ege6206k70509a3cgk7npn3plg7r8 |



## Tenderseeds

We operate Tenderseed instances for every #ibcgang blockchain on Akash.

You can connect to them here:







## Multi-chain Port Standard




Each chain has 10 ports it can use.  WIP.


| Network      | Port Range | 
| ----------- | ----------- | 
| Osmosis   | 2000-2009   | 
| Gaia      | 2010-2019   | 
| Akash     | 2020-2029   | 
| Sentinel  | 2030-2039   | 
| Crypto.org | 2040-2049  | 
| Regen      | 2060-2069  | 
| Omniflix  | 2070-2079 |
| Juno       | 2050-2059 |
| Starname   | 2130-2139   | 
| Iris       | 2120-2129   | 
| Persistence| 2080-2089  | 
| dig        | 2090-2099 |

| Service      | Port  | 
| ----------- | ----------- | 
| p2p   | xxx0  |
| rpc   | xxx1  |
| grpc  | xxx2 |
| api   | xxx3 |
| grpc-web | xxx4 |
| load balanced rpc | xxx9 |



# Products
All of Notional's products are 100% open source, though some do have unusal licenses.

* [SOS](https://github.com/notional-labs/sos) Lightweight operating system based on Arch Linux
* [Archlinux-Docker](https://github.com/faddat/archlinux-docker) Arm64/amd64 multiplatform docker image for Arch
* [Validatron](https://whimsical.com/validatron-PbUypC8tVMU8DxCFNLdDFu) designs and equipment for edge validation
* [ipfsync](https://github.com/notional-labs/ipfscync) IPFS collaborative cluster enabling syncs that saturate a 10gbps line
* [tradeberry](https://github.com/notional-labs/tradeberry) Raspberry pi image that allows private usage of Osmosis
* [dig](https://github.com/notional-labs/dig) Liquid Land


We have been working with https://pcbviet.com on open source hardware, and hope to run tradeberry on a Minimus PC sometime in 2021.

## Team
* Jacob Gadikian - Blockchain and infrastructure engineer
* Ricardo Ferreria - All things biz, testing of documentation written by Jacob and Khanh
* Khanh Nguyen - Blockchain Engineer
* Minh Vu Le Nhat - Hermes Operator 

**Notional is hiring and training blockchain engineers.  Hours are ludicrous, and all team members earn a meaningful stake in all blockchains launched.  Notional Pays flat global wages.** 

## Technical Partnerships with other validators / relayers
* https://github.com/chandrastation

Our technical partners agree to:
* Mutual Aid Re: Uptime (eg: phone calls to one another)
* Full commitment to open source, repeatable infrastructure (we only partner with validators who document their infrastructure)
* Join a Signal chat, since it's not discord
* Share information about chain launches




## Thanks
Notional would like to thank its delegagtes and the many teachers who have helped us learn how to design and implement all of this.

Special thanks go out to:

* PCBViet
* Chandra Station
* DefiForYou
* Osmosis Team & Community
* Jae Kwon & Gno Community
* Shakti Open Semiconductor Project
* Jack Zampolin & Strangelove Ventures