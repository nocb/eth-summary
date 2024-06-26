


### 书籍：

https://www.gitbook.com/book/easonwang01/blockchain/details



### eth猫 
https://www.cryptokitties.co/kitty/83194

源码
https://github.com/axiomzen/cryptokitties-bounty

### eth猫源码说明
http://ethfans.org/posts/how-to-code-your-own-cryptokitties-style-game-on-ethereum

### 合约反编译

https://github.com/comaeio/porosity


### eth浏览器 

https://ethplorer.io

https://etherscan.io/ 

https://www.etherchain.org/

api调用   https://etherscan.io/apis

### eth浏览器源码

https://github.com/gobitfly/erc20-explorer

https://github.com/gobitfly/etherchain-light

### 以太坊节点状态统计
https://www.ethernodes.org/network/1

https://stats.ethfans.org/     星火计划

###  以太坊状态 到底设置多少 gas price 合适 ，整个以太坊的情况，并给你建议的 gas price。

https://ethgasstation.info/

### EVM 说明

EVM（Ethereum Virtual Machine, 以太坊虚拟机）是以太坊的核心，负责运行智能合约和处理交易。是一个计算引擎，提供了计算和存储的抽象，类似于 Java 虚拟机 （JVM） 规范。EVM 执行自己的字节码指令集，这些指令集通常由 Solidity 编译而成。
- EVM的执行指令都是需要耗费gas的，避免出现死循环，区块之间是有关联的，下一个区块依赖上一个区块的状态，所以以太坊的串行执行，很难做并行优化。 
- 以太坊协议约定交易按照顺序执行。虽然顺序执行确保了交易和智能合约能够以确定性顺序执行，保障了安全性，但在面临高负载的情况下，可能会导致网络拥堵和延迟，这也是为什么以太坊有极大的性能瓶颈，需要 Layer2 Rollup 扩容的原因。
- EVM 设计成一台256位的虚拟机，未来可优化为 WASM 或 Move字节码的虚拟机，
- EVM 实现并行执行的主要挑战是确定哪些交易是不相关的，哪些是独立的。 
- 并行 EVM（Parallel EVM）， 产品有：
    - Monand  
    - Sei V2 
    - Artela
    - Solana Neon
- 参考：https://learnblockchain.cn/article/7842
