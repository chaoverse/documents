# chaoverse 文档

## chaoverse 是什么？

chaoverse 初步定义并行于 [Chao Art Dao](https://opensea.io/collection/untitled-collection-238952168) 的DAO 组织。

## 初步规划

社区以 Chao Art Dao 发行的NFT 为主要载体，通过智能合约完成 NFT 的 销毁、置换、赋能 等一系列操作。

社区最终形态，以智能合约的方式独立运行，社区的行为通过操作智能合约来完成。 社区成员通过投票决定 智能合约的走向。（路漫长，不过值得期待）

## 已完成合约及部分说明

* chaoverse.base

NFT 基础合约,Chao Art Dao 在 Polygon 上发布的所有NFT 记录。
0x3204A08dBA306081ef7622bEa6A30cC1f66E929c
<https://polygonscan.com/address/0x3204A08dBA306081ef7622bEa6A30cC1f66E929c#code>

* chaoverse.burnner NFT  燃烧合约基础版
0x0a4c233a54a22aB8620C589819Ea3DC5A814473a
<https://polygonscan.com/address/0x0a4c233a54a22aB8620C589819Ea3DC5A814473a#code>

## 新燃烧合约 (测试中)

0xDC0cf8E947220aE047B87e2c2a39782736421290
在原有燃烧合约的基础上，发放一定的碎片。用于奖池的兑换。

碎片发放分两种:

1. 普通用户 0
2. 持有五个 burnner nft 或者 自画像的燃烧用户 发放1个碎片
3. 销毁发起者发放 burn_count 个 nft (后期随着合约完善，销毁活动会下放到各个OG)

关于NFT 碎片

NFT 碎片属于一种销毁凭证，类似于超市里的购物小票积分。 兑换过程类似于 超市里的积分兑换。
NFT 碎片最终流向
奖池合约 --> 销毁合约 --> 销毁用户 或 销毁活动发起者-> 回到奖池合约

## 碎片兑换奖池 (测试中)

0xE8423E4324a67af4D405584e07c39C69C22C8560

1. 持有五个 burnner nft 或者 自画像的燃烧用户 通过消耗一定的碎片获取 nft
2. 碎片兑换完成后，回到奖池合约
3. 可以取回碎片或者奖励 nft
