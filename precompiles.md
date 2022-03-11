# EVM 预编译合约

本文内容参考自：

- https://github.com/ethereum-optimism/optimism/blob/develop/l2geth/params/protocol_params.go
- https://github.com/ethereum-optimism/optimism/blob/develop/l2geth/core/vm/contracts.go

虽然很方便，但是最好还是访问 geth 仓库。

以下数额均为 Istanbul 版本：

| Address | Name           |   Gas   | Notes |
| :-----: | :------------- | :-----: | :---- |
|  0x01   | ecrecover      |  3000   |       |
|  0x02   | sha256hash     | Dynamic |       |
|  0x03   | ripemd160hash  | Dynamic |       |
|  0x04   | dataCopy       | Dynamic |       |
|  0x05   | bigModExp      | Dynamic |       |
|  0x06   | bn256Add       |   150   |       |
|  0x07   | bn256ScalarMul |  6000   |       |
|  0x08   | bn256Pairing   | Dynamic |       |
|  0x09   | blake2F        | Dynamic |       |

Berlin 版本似乎没有修改数值。
