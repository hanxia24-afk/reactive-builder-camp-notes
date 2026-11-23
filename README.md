# Reactive Builder Camp 学习记录

## 环境准备

- 测试钱包：`0xC2a5E7D5715b3c5536C22f0992F3BDD22842b8dE`
- [Lasna 钱包及 lREACT 余额](https://lasna.reactscan.net/address/0xC2a5E7D5715b3c5536C22f0992F3BDD22842b8dE)
- WSL2 Ubuntu，Foundry forge 1.9.0；本地测试 8 项通过。

## 2026-11-16：跨链回调

完成 Sepolia → Lasna → Sepolia 跨链流程：

1. [Sepolia Ping 事件交易](https://sepolia.etherscan.io/tx/0x8dc2e488cdf1a576d3f9f174dcfa6314be50d467d9b2449a50bf7687e519b507)
2. [Lasna Reactive 合约](https://lasna.reactscan.net/address/0xa8315d026DC30746dE74157fc03922dea0F6286A)：源交易哈希与 Ping 一致，lastReactBlock 为 8490529。
3. [Sepolia Handled 回调交易](https://sepolia.etherscan.io/tx/0x1d88afe8831622572ec83595b7fd3edbf0226d1a02a8ec7dd9fc8c9db47cdee4)：count 为 1，lastValue 为 500。

该账户仅用于测试网。
