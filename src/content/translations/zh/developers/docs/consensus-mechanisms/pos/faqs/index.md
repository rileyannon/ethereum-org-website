---
title: 常见问题
description: 常见问题：权益证明以太坊
lang: zh
---

## 权益证明是什么？ {#what-is-proof-of-stake}

权益证明是一种算法类别，通过确保攻击者因欺诈行为而损失有价值的资产，可以为区块链提供安全性。 权益证明系统需要一组验证者提供一些资产，如果验证者从事某些被证明为欺诈的行为，则可以销毁这些资产。 以太坊使用权益证明机制来保护区块链的安全性。

## 权益证明与工作量证明相比有何不同？ {#comparison-to-proof-of-work}

权益证明和工作量证明都是从经济上抑制恶意行为者的机制，以防止其向网络发送垃圾或进行欺诈行为。 在两种情况下，积极参与共识的节点都会“向网络中”投入某些资产，如果他们行为不当，便会失去这些资产。

在工作量证明中，这种资产是能源。 节点，也称为矿工，会运行一个算法，目的是比任何其他节点更快地计算出一个值。 最快的节点有权向链中提议一个区块。 要更改链的历史记录或主导区块提议，矿工必须拥有足够的算力，以便它们始终赢得比赛。 由于代价高昂且执行难度极大，这一过程保护了区块链免受攻击。 使用工作量证明挖矿所需的能源是矿工支付的现实世界资产。

权益证明要求节点（称为验证者）向智能合约明确提交一种加密资产。 如果验证者行为不当，这种加密货币可以被销毁，因为他们是将自己的资产直接质押到链中而不是通过能量消耗的方式间接质押。

工作量证明需要在挖矿过程中消耗大量的电力，因此能耗要高得多。 而权益证明只需要非常少量的能量 - 以太坊验证者甚至可以在树莓派等低功耗设备上运行。 以太坊的权益证明机制被认为比工作量证明机制更安全，因为攻击的代价更高，并且给攻击者造成的后果更严重。

工作量证明与权益证明是一个有争议的话题。 [Vitalik Buterin 的博客](https://vitalik.ca/general/2017/12/31/pos_faq.html#what-are-the-benefits-of-proof-of-stake-as-opposed-to-proof-of-work)以及 Justin Drake 与 Lyn Alden 之间的辩论对这些论点做了很好的总结。

<YouTube id="1m12zgJ42dI" />

## 权益证明的能效高吗？ {#is-pos-energy-efficient}

由此可见， 权益证明网络上的节点能耗很低。 一项第三方研究得出的结论是，整个基于权益证明的以太坊网络每年消耗约 0.0026 亿千瓦时的电量，仅相当于美国博彩行业电力消耗量的 1/13000 左右。

[关于以太坊能源消耗的更多信息](/energy-consumption/)。

## 权益证明安全吗？ {#is-pos-secure}

以太坊的权益证明是非常安全的。 这种机制经过了八年的研究、开发和严格测试，才得以投入使用。 安全保证有别于使用工作量证明的区块链。 在权益证明机制中，可以主动惩罚（“罚没”）恶意验证者并将其从验证者组中驱逐出去，这将导致其损失大量的以太币。 而在工作量证明中，攻击者在拥有足够哈希能力的情况下可以不断重复攻击。 与工作量证明以太坊相比，对权益证明以太坊发起同等攻击的成本也更高。 要影响链的活性，至少需要网络上已质押以太币总数的 33%（除非进行极为复杂、成功概率极低的攻击）。 要控制未来区块的内容，至少需要已质押以太币总量的 51%，而要重写历史记录，则需要超过质押总量的 66%。 以太坊协议将在 33% 或 51% 攻击场景中销毁这些资产，并通过社会共识来应对 66% 攻击场景。

- [关于保护以太坊权益证明机制免受攻击的更多信息](/developers/docs/consensus-mechanisms/pos/attack-and-defense)
- [关于权益证明设计的更多信息](https://medium.com/@VitalikButerin/a-proof-of-stake-design-philosophy-506585978d51)

## 权益证明机制降低了以太坊的费用吗？ {#does-pos-make-ethereum-cheaper}

否。 发送交易的成本（燃料费）由动态费用市场决定，随着网络需求的增加而增加。 共识机制对此没有直接影响。

[关于燃料的更多信息](/developers/docs/gas)。

## 什么是节点、客户端和验证者？ {#what-are-nodes-clients-and-validators}

节点是连接到以太坊网络的计算机。 客户端是在计算机上运行，将其转化为节点的软件。 有两种类型的客户端：执行客户端和共识客户端。 两种客户端都是创建节点所需的。 验证者是共识客户端一个可选的附加功能，使节点能够参与权益证明共识。 这意味着当被选中时创建和提议区块，以及认证其在网络上监听到的区块。 要运行验证者，节点运营商必须在存款合约中存入 32 个以太币。

- [关于节点和客户端的更多信息](/developers/docs/nodes-and-clients)
- [关于质押的更多信息](/staking)

## “权益证明”是一个新的概念吗？ {#is-pos-new}

否。 早在 2011 年，BitcoinTalkk 论坛上有一位用户就[提出了将权益证明作为比特币的升级形态的想法](https://bitcointalk.org/index.php?topic=27787.0)。 11 年后，才准备好在以太坊主网上实施。 一些其他的区块链比以太坊更早实施了权益证明，但不是以太坊的特定机制（称为 Gasper）。

## 以太坊的权益证明有什么特别之处？ {#why-is-ethereum-pos-special}

以太坊的权益证明机制在其设计上是独一无二的。 它不是第一个设计和实施的权益证明机制，但它是最完善的。 该权益证明机制被称为“Casper”。 Casper 定义了如何选择验证者来提议区块、如何及何时进行认证、如何计数认证、给予验证者的奖励和惩罚、罚没条件、故障转移机制（如“怠惰惩罚”），以及“最终确定性”的条件。 最终确定性是指一个区块被认为是规范链的永久部分的条件，即它必须得到网络上已质押的以太币总量至少 66% 的投票。 研究人员专门为以太坊开发了 Casper，以太坊是第一个也是唯一一个实现了它的区块链。

除了 Casper，以太坊的权益证明还使用了一种叫做 LMD-GHOST 的分叉选择算法。 这是在出现两个区块存在于同一个时隙的情况下所需的。 这会创建区块链的两个分叉。 LMD-GHOST 选择具有最大认证“权重”的分叉。 权重是指按验证者有效余额加权后的认证数量。 LMD-GHOST 是以太坊独有的。

Casper 和 LMD_GHOST 的组合被称为 Gasper。

[关于 Gasper 的更多信息](/developers/docs/consensus-mechanisms/pos/gasper/)

## 什么是罚没？ {#what-is-slashing}

罚没是指销毁验证者的部分质押额并将验证者从网络中逐出的行为。 罚没中损失的以太币数量随着被罚没的验证者数量而变化 - 这意味着串通的验证者会受到比个人更严厉的惩罚。

[关于罚没的更多信息](/developers/docs/consensus-mechanisms/pos/rewards-and-penalties#slashing)

## 为什么成为验证者需要质押 32 个以太币？ {#why-32-eth}

验证者必须质押以太币，这样他们就有了当行为不当时便会损失的东西。 之所以要质押 32 个以太币，是为了让节点能够在适度的硬件上运行。 如果每个验证者的最少以太币数量更低，那么验证者的数量，继而每个时隙必须处理的消息数量就会增加，而这意味着需要更强大的硬件来运行节点。

## 验证者是如何被选中的？ {#how-are-validators-selected}

每个时隙都会以伪随机的方式选择一个验证者来提议区块，使用的算法被称为 RANDAO，它将区块提议者的哈希与一个随每个区块更新的种子混合在一起。 这个值用于在所有验证者中选择一个特定的验证者。 验证者的选择会提前四个时段固定。

[关于如何选择验证者的更多信息](/developers/docs/consensus-mechanisms/pos/block-proposal)

## 什么是权益粉碎攻击？ {#what-is-stake-grinding}

权益粉碎攻击是针对权益证明网络的攻击类别，这种情况下，攻击者试图将验证者选择算法偏向于选择他们自己的验证者。 对 RANDAO 发起权益粉碎攻击需要已质押的以太币总数的约一半。

[关于权益粉碎攻击的更多信息](https://eth2book.info/altair/part2/building_blocks/randomness/#randao-biasability)

## 什么是社交罚没？ {#what-is-social-slashing}

社交罚没是指社区协调区块链的分叉以应对攻击的能力。 它使社区能够从攻击者最终化不诚实的链中恢复过来。 它也可以用于对抗审查攻击。

- [关于社交罚没的更多信息](https://ercwl.medium.com/the-case-for-social-slashing-59277ff4d9c7)
- [Vitalik Buterin 关于社交罚没的观点](https://vitalik.ca/general/2017/12/31/pos_faq.html#what-is-proof-of-stake)

## 我会受到罚没吗？ {#will-i-get-slashed}

作为验证者，除非您故意从事恶意行为，否则不会受到罚没。 罚没机制只会在极其特定的情况下实施，比如验证者在同一时隙提议多个区块或者在其认证中出现自相矛盾等行为，这类情况很少会在正常操作中意外发生。

[关于罚没条件的更多信息](https://eth2book.info/altair/part2/incentives/slashing)

## 什么是无利害关系问题？ {#what-is-nothing-at-stake-problem}

无利害关系问题是一些权益证明机制中的一个概念性问题，其中只有奖励而没有惩罚。 如果没有任何利害关系，那么一个务实的验证者同样愿意验证任何甚至多个区块链分叉，因为这将增加他们的奖励。 以太坊通过使用最终确定性条件和罚没机制来确保只有一个规范链，以解决此问题。

[关于无利害关系问题的更多信息](https://vitalik.ca/general/2017/12/31/pos_faq.html#what-is-the-nothing-at-stake-problem-and-how-can-it-be-fixed)

## 什么是分叉选择算法？ {#what-is-a-fork-choice-algorithm}

分叉选择算法实施规则，确定哪条链是规范链。 在最优条件下，没有必要使用分叉选择规则，因为每个时隙只有一个区块提议者和一个可供选择的区块。 但是，偶尔会出现同一个时隙内有多个区块或者由于晚到的信息导致链头附近的区块组织方式存在多个选择的情况。 在这些情况下，所有客户端都必须以相同的方式执行一些规则，确保它们都选择正确的区块序列。 分叉选择算法的代码中体现了这些规则。

以太坊的分叉选择算法被称为 LMD-GHOST。 它会选择具有最大认证权重的分叉，也就是得到了最多质押以太币投票的分叉。

[关于 LMD-GHOST 的更多信息](/developers/docs/consensus-mechanisms/pos/gasper/#fork-choice)

## 什么是权益证明中的最终确定性？ {#what-is-finality}

权益证明中的最终确定性是指保证给定的区块是规范链的永久部分，并且只有在出现共识失败的情况下才会被回滚，这时攻击者将会销毁已质押以太币总数的 33%。 这是“加密经济”的最终确定性，而不是与工作量证明区块链相关的“概率最终确定性”。 在概率最终确定性中，区块没有明确的确定/非确定状态——只不过随着时间的推移，区块从链上被删除的可能性越来越小，用户将自行决定他们什么时候有足够的信心认为区块是“安全的”。 而在加密经济的最终确定性下，成对的检查点区块必须获得已质押以太币 66% 以上的选票。 如果满足这个条件，这两个检查点之间的区块将被明确“最终确定”。

[关于最终确定性的更多信息](/developers/docs/consensus-mechanisms/pos/#finality)

## 什么是“弱主观性”？ {#what-is-weak-subjectivity}

弱主观性是权益证明网络的一个特点，其中社交信息用于确认区块链的当前状态。 新节点或长时间离线后重新加入网络的节点可以获得最新的状态，以便节点能够立即查看它们是否位于正确的链上。 这些状态被称为“弱主观性检查点”，它们可以从其他带外节点运营者处获取，也可以从区块链浏览器或多个公共端点获取。

[关于弱主观性的更多信息](/developers/docs/consensus-mechanisms/pos/weak-subjectivity)

## 权益证明能抗审查吗？ {#is-pos-censorship-resistant}

抗审查性当前很难证明。 然而，与工作量证明不同，权益证明提供了协调罚没以处罚审查验证者的选择。 该协议即将修改为将区块构建者与区块提议者分开，并实施构建者必须在每个区块中包括的交易列表。 此提案被称为“提议者-构建者分离”，有助于防止验证者审查交易。

[关于“提议者-构建者分离”的更多信息](https://notes.ethereum.org/@fradamt/H1TsYRfJc#Original-basic-scheme)

## 以太坊的权益证明系统会受到 51% 攻击吗？ {#pos-51-attack}

由此可见， 权益证明和工作量证明一样，容易受到 51% 攻击。 攻击者不需要掌控 51% 的网络算力，而是需要掌控已质押以太币总数的 51%。 如果攻击者累积了总质押量的 51％，则能够控制分叉选择算法。 这使得攻击者能够审查某些交易，进行短程重组，以及通过以有利于他们的方式重新排序区块来提取矿工可提取价值。

[关于权益证明攻击的更多信息](/developers/docs/consensus-mechanisms/pos/attack-and-defense)

## 什么是社交协调，为什么需要它？ {#what-is-social-coordination}

社交协调是以太坊的最后一道防线，它可以使一个由于遭到攻击而最终化了不诚实区块的区块链恢复到诚实状态。 在这种情况下，以太坊社区将不得不进行“带外”社交协调并同意使用诚实的少数分支，同时罚没攻击者的验证者。 这需要应用程序和交易所也认可诚实的分叉。

[了解关于社交协调的更多信息](/developers/docs/consensus-mechanisms/pos/attack-and-defense#people-the-last-line-of-defense)

## 在权益证明中，富人会变得更富有吗？ {#do-rich-get-richer}

将越多的以太币用于抵押，一个人就能运行越多的验证者，也能获得更多的奖励。 奖励与抵押的以太币数量成线性比例，每个人获得相同百分比的回报。 工作量证明比权益证明更能让富人富裕起来，因为大规模购买硬件的富裕矿工将受益于规模经济，这意味着财富和奖励之间的关系是非线性的。

## 权益证明是否比工作量证明更中心化？ {#is-pos-decentralized}

不，由于采矿成本增加、价格高昂迫使个人和小公司退出等原因，工作量证明更倾向于集中化。 目前权益证明存在的问题是流动性质押衍生品的影响。 这些是代表某些提供者所质押的以太币的代币，任何人都可以在二级市场上交换，而无需实际解除以太币的质押。 流动性质押衍生品允许用户质押的以太币数量少于 32 个，但也会产生中心化风险，即少数几个大型组织最终可能控制大部分的质押份额。 这就是为什么[单独质押](/staking/solo)成为以太坊的最佳选择。

[关于流动性质押衍生品中的权益中心化的更多信息](https://notes.ethereum.org/@djrtwo/risks-of-lsd)

## 为什么我只能质押以太币？ {#why-can-i-only-stake-eth}

ETH 是以太坊的原生货币。 为计算有效余额以用于加权投票和确保安全性，必须有一种单一的货币来计量所有权益。 以太币本身是以太坊的一个基本组成部分，而不是一个智能合约。 如果加入其他货币，将会显著增加质押的复杂性并降低其安全性。

## 以太坊是唯一使用权益证明的区块链吗？ {#is-ethereum-the-only-pos-blockchain}

不，现在有多种使用权益证明的区块链。 但是没有一个和以太坊完全相同；以太坊的权益证明机制是独一无二的。

## 什么是合并？ {#what-is-the-merge}

合并是指以太坊关闭其基于工作量证明的共识机制并开启其基于权益证明的共识机制的时刻。 合并发生在 2022 年 9 月 15 日。

[关于合并的更多信息](/roadmap/merge)

## 什么是活性和安全性？ {#what-are-liveness-and-safety}

活性和安全性是区块链的两个基本安全问题。 活性是指最终链的可用性。 如果链停止最终化或用户无法轻松访问它，这些都是活性失败。 极高的访问成本也可能被认为是一种活性失败。 安全性是指攻击链，即最终化彼此冲突的检查点的难度有多大。

[阅读关于 Casper 论文的更多信息](https://arxiv.org/pdf/1710.09437.pdf)