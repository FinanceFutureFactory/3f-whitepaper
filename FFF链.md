# Finance Future Factory链

> 支持智能合约的Finance Future Factory链

1.0版本

2022/09/07

- [特色](#特色)
- [资产挂钩黄金](#资产挂钩黄金)
- [实体资产上链](#实体资产上链)
- [构建WEB3 DAPP ](#构建WEB3 DAPP )
- [设计原则](#设计原则)
- [共识与验证者的人数](#共识与验证者的人数)
  - [基于权益的权威证明 (Proof Of Staked Authority)](#基于权益的权威证明-proof-of-staked-authority)
  - [验证人节点法定人数](#验证人节点法定人数)
  - [安全与最终性](#安全与最终性)
  - [收益](#收益)
- [代币经济学](#代币经济学)
  - [原生代币](#原生代币)
  - [其他代币](#其他代币)
- [权益质押](#权益质押)
  - [FFF权益质押](#FFF权益质押)
  - [奖励](#奖励)
  - [罚息](#罚息)
- [中继器](#中继器)
  - [FFF中继器](#FFF中继器)
    - [激励](#激励)
  - [Oracle中继器](#oracle中继器)
- [展望](#展望)

## 特色
FFF资产链是由Finance Future Factory 开发团队创立，旨在创新实践以黄金为计量单位的实体资产挂钩的公链，其新颖的实体资产的采用和发展，结合区块链独有的NFT和token推出Web3 dApp 的首屈一指的扩展解决方案。
## 资产挂钩黄金
通货膨胀是能够造成主要商品的物价持续、普遍、不可逆的上涨。另一方面则是本币贬值，货币的购买力不断下降。通货膨胀就是市面上流通的货币越来越多，而货物增量跟不上货币的增量，于是货币越来越不值钱。在布雷顿森林体系破灭后，现在全球贸易体系都是以美元作为结算的，这其中美元又和汇率挂钩，但是美国政府和各个国家的政府都无法抑制住自己印钱的冲动，导致货币不断贬值。
FFF资产链的设立目标是真实资产上链，并且以黄金本位代币EURCO作为计价单位，EURCO是以锚定黄金价值目标的本位代币，所以EURCO不受到通货膨胀的影响，不会因为政府印钱导致代币价值贬值

## 实体资产上链
FFF资产链是以区块链为技术开发全新的NFT体系，每一个NFT拥有独一无二的id，FFF资产链允许每一个NFT可以挂钩实体资产，例如房产、珠宝黄金、游艇的实体支撑。实体资产上链后被铸造成为NFT，重新塑造NFT的真实价值，不再是虚拟的NFT。Finance Future Factory 研发FFF资产链致力于把新颖的实体资产转换为数字化资产，实现数字化金融的升级

## 构建WEB3 DAPP 
FFF资产链也是一个用于去中心化应用程序的开放、可编程的智能合约平台，允许全世界的开发者参与构建WEB3 DAPP应用，即时确认交易并每秒处理数千笔交易，远超当今任何去中心化区块链平台。开发者以极低的成本，快速，安全，高效的构建与实体资产挂钩的应用，通过黄金计价代币EURCO作为底层计价货币，形成一套全新的金融体系。

## 设计原则

在FFF链生态系统中构建的区块链被称为“FFF链”（以下部分简称为**“FFF”**）。

FFF的设计遵循以下原则：

1. **独立区块链**： 从技术上讲，FFF 是一个独立的区块链，而不是Layer 2解决方案。 FFF 的基础技术和业务功能是独立的。

2. **以太坊兼容**： 第一个实用的、被广泛使用的智能合约平台是以太坊 。为了对接相对成熟的应用和社区，FFF 选择与现有的以太坊主网兼容。 这意味着大多数**dApp**、生态系统组件和工具将与FFF兼容，不需要修改或只需要很小的更改；FFF 节点仅需要类似，或稍高的硬件规范和操作技能就能运作。这一实现应为 FFF 和以太坊未来的版本继续兼容提供空间。

3. **基于权益质押的共识和链上管理的**：基于权益质押（PoS）的共识更环保，给社区治理提供更灵活的选择。可以预期的是，这种共识会比PoW共识有更好的性能，即出块时间短，交易处理容量高。

## 共识与验证者的人数

基于以上设计原则，FFF的共识协议是为了实现以下目标：
1. 出块时间应该比以太坊时间短，例如 3 秒甚至更短。
2. 只需要等待有限的时间就能最终确认交易，例如大约 30 秒或更短。
3. 没有通货膨胀，区块链的收益来自手续费，手续费以FFF-Coin的形式支付。
4. 尽可能与以太坊兼容。
5. 配备了基于权益质押机制。

### 基于权益的权威证明 (Proof Of Staked Authority)

尽管工作量证明（PoW）已被证明为实现去中心化网络的实用方案，但它对环境并不友好，而且还需要大量参与者来维护网络安全。

以太坊及一些其他网络，如 MATIC Bor、TOMOChain、GoChain、xDAI在不同的场景中使用权威证明（PoA）或其变体，包括测试网络和主网。PoA 为 51%的攻击提供了防御，更有效的防止一部分拜占庭节点作恶。 选用PoA作为底层共识是理想的选项之一。

同时，PoA 协议因不如PoW去中心化而被批评，因为验证人，即轮流生成块的节点，拥有极大的权力，并且容易产生腐败和遭受安全攻击。 其他区块链, 如 EOS, 引入了不同类型的委托权益证明（DPoS），允许代币持有者投票选举验证人节点。 它让网络更加去中心化，有利于社区管理。

受以上启发，FFF 将 DPoS 和 PoA 结合以达成共识，采用的方案为：

1. 区块是由有限数量的验证人生成的
2. 验证人轮流以     PoA 方式生成区块，类似于以太坊的Clique共识引擎
3. 验证人集合是基于权益质押的链上治理选出和淘汰

### 验证人节点法定人数

在网络启动的创世块阶段，一些受信任的节点将作为初始验证人集合运行。开始出块后，任何人都可以作为候选人参与竞选验证人。 权益质押状态决定前 5 个权益质押最多的节点成为下一个验证人集合，这样的选举和淘汰每 24 小时进行一次。

**FFF-coin 是FFF权益质押的通证。**

在生成新的区块前，现有的FFF验证人定期检查是否有`“ValidatorSetUpdate”`消息转发到FFF 。 如果有，它们将在一段高度后（即预定义的区块间隔）之后更新验证人集合。 例如，如果 FFF 每 3 秒生成一个区块且检查周期是 200 个区块，那么当前的验证人集合将在 600 秒（10 分钟）内检查并更新下一周期的验证人集。

### 安全与最终性

考虑到有超过一半的 ½\*N+1 验证人是诚实可信的，基于 PoA 的网络通常可以安全、正常地工作。 然而在某些情况下，拜占庭验证人仍然可能设法攻击网络， 比如通过“克隆攻击”的方式。 为了保证具FFF有与BTC,ETH一样高的安全性，我们鼓励FFF 用户等待到接收的区块被超过⅔\*N+1 不同的验证人所确认。 通过这种方式，FFF 可以实现与 BTC,ETH 相似的安全级别，可以容忍少于1/3 \*N 的拜占庭验证人。

对于 5 个验证人，如果区块时间为 3 秒，那么 ⅔\* N + 1 个不同的验证人确认将需要（2/3\*5 + 1）\*3 =12秒的时间。FFF 的任何重要应用程序可能都必须等待⅔*N + 1，以确保相对安全的最终结果。 然而，除了这样的安排，FFF 还引入了惩罚机制来惩罚拜占庭验证人的双重签名或不稳定性，这将在后面的“权益质押和管理”部分中做出介绍。 这种惩罚机制将在很短的时间内暴露恶意验证人，并使 “克隆攻击”非常难以执行或即使执行了也非常不划算。 通过这种惩罚机制，½\*N + 1 甚至更少的区块就足够满足大部分交易最终性了。

### 收益

当前验证人集合中的所有 FFF 验证人都将从以FFF-coin 支付的手续费中获得收益。由于 FFF-coin 不是一个会通胀的通证，因此不会像比特币和以太坊网络那样产生挖矿收益，手续费是验证人的主要收益。 由于FFF-coin 也是其他应用的实用型通证，委托人和验证人仍将获得持有FFF-coin 的其他好处。

验证人的收益是从每个区块的交易中收取的手续费获得的。验证人可以决定向质押了FFF-coin 的委托人分享多少收益，以吸引更多的质押投资。 每个验证人将以相同的概率轮流生成区块（如果它们保持 100%在线），因此，从长远来看，所有稳定的验证人都可能获得类似规模的收益。 同时，每个验证人的质押资产大小可能是不同的，因此，这带来了一种与直觉相反的情况，即更多的用户信任并委托质押于同一个验证人，他们可能获得更少收益。因此，只要验证人仍然是可信的（不受信任的验证人可能带来极大的风险），理性的委托人就会倾向于委派抵押数量较低的验证人。 最终，所有验证人的区别都会更小。这实际上将防止其他网络上出现的质押集中和“赢家永远赢”的问题。

### 原生代币

FFF-coin在FFF上运行的方式与ETH 在 以太坊 上运行的方式相同，因此它是FFF的“原生代币”。这意味着FFF-coin 除了可以在FFF链或者3FEX上被用来支付大部分手续费用之外，FFF-coin 也将用于：

1.支付在 FFF上部署智能合约的手续费
2.对选定的 FFF 验证人进行权益质押，并获得相应的奖励

### 其他代币

FFF 支持 FRC20代币，它们是原生资产，可快速交易并确认，可以流通，上币后可以在3FEX上交易。 同时，由于 FFF 是 以太坊兼容的，在 FFF 上支持 ERC20合约被称为 “FRC2E”（未来可以通过FRC修改命名）。FRC2E通过添加更多的方法来“增强”已有协议，这些方法可以公开更多的信息，比如代币单位、精度。 FFF确保一个代币在不同的用例中的总流通量不变。

## 权益质押

PoSA实现了去中心化式的社区治理。 你可以从其他网络中看到类似的想法，特别是 Cosmos 和 EOS 。 其核心逻辑可概括如下。

1. 代币持有者，包括验证人，可以将他们的代币 “锁定”到权益质押中。 代币持有者可以将他们的代币**委托**给任何验证人或一个验证人候选对象。 之后他们还可以重新选择不同的验证人或候选对象来对他们的代币进行委托。
2. 所有验证人候选对象都将按其获得委托代币的数量进行排序，排名前列的将成为真正的验证人。
3. 验证人可以与它们的委托人共享区块收益。
4. 验证人可能会遭受**“罚息”**，即对他们的不良行为的惩罚，如双重签名和/或不稳定性。 这样的损失也会与他们的委托人共同分担。
5. 验证人和委托人有一个 “解除绑定期”。当发现恶意拜占庭行为时，代币仍然在一定时间内保持锁定，作恶人将被及时惩罚。


### FFF权益质押

理想情况下，这样的权益质押和奖励发放逻辑应该包含在区块链中，并在产生新区块时自动执行。与币安链一样采用Tendermint共识库的Cosmos Hub就是这样工作的。

自设计之日起，FFF就一直在准备启用PoS。另一方面，FFF想要尽可能地与以太坊保持兼容，在其上直接实现PoSA是一个巨大的挑战和压力。特别是考虑到以太坊本身可能在短时间（或更长时间）内迁移到PoS共识协议时，尤其如此。为了保持以太坊的兼容性和复用FFF的基础架构，我们在FFF上完成了权益质押逻辑：

1. 质押代币是 FFF-coin，这是因为它是FFF链上的原生代币。
2. 在FFF上记录FFF的权益质押和委托行为。
3. FFF 验证人集由它的权益质押和委托逻辑来决定，在FFF上构建一个FFF的权益质押模块，并通过通信在每天UTC 00:00:00 传送到 FFF 。
4. FFF上的奖励分配发生在每天UTC 00:00时刻。

### 奖励

验证人集更新和奖励分配都发生在每天 的UTC 00:00 。这是为了节省频繁更新和区块奖励分配的成本。频繁分配奖励的代价可能是巨大的，因为区块奖励是在FFF上收取的，并在FFF上分发给FFF验证人和委托人。（请注意，FFF出块奖励仅分发给FFF验证人。）

为了确保分配是公平的，这里引入了一种延后分配的算法：

1. 区块奖励不会立即发送给验证人，而是计算并积累在智能合约中；
2. 当FFF收到验证人集更新消息时，它将触发转账，将奖励转账给验证人的托管地址。 托管地址是由系统控制，因此在向委派者承诺的分配完成之前，奖金是不能用的。
3. 为了使同步更简单，并分配时间以防出现罚没，第T天的奖励将在第T + 2 天分配。 在委托人收到奖励后，剩下的收益将被转移到验证人自己的奖励地址。

### 罚息

罚息是链上管理的一部分，以确保恶意或负面行为受到惩罚。 FFF罚息证据可以由任何人提交。 交易提交要求提交罚息证据和缴纳手续费，但一旦成功提交，也带来了更多奖励。

到目前为止，有两种可以被惩罚的情况。

**双重签名**

当验证人故意签署多个相同高度并具有相同父块的区块时，这是很严重的作恶行为。 协议的实现应该已经考虑到如何防止这种情况发生，因此只有恶意代码才能触发这种情况。当出现双重签名时，验证人应该立即从验证人集合中移除。

任何人都可以在 FFF 上提交带有 FFF 双重签名的罚息请求，应该包含两个具有相同高度的区块头和母区块，以及违规验证人的签名。 在收到证据后，如果 FFF 确认该证据是有效的：

1. 该验证人将立刻发送 FFF “验证人集合更新”消息，恶意验证人将从验证集中剔除；
2. 验证人的权益质押将按照预先设定的金额进行惩罚；
3. 一部分被惩罚的FFF-coin 将奖励给证据提交者。奖励金额应远远大于提交罚息请求事件的成本
4. 剩下的 FFF-coin 将分配给其他验证人的托管地址，并以与区块奖励相同的方式分配给所有委托人。

**不稳定性**

FFF 的可用性依赖于PoSA共识中验证人集合中的每个验证人，当轮到其出块时，他们能够及时生成区块。 验证人可能由于一些原因而错过出块时机，特别是由于硬件、软件、配置或网络方面的问题。 这种不稳定运行将损害网络的性能，并给系统带来更多的不确定性。

FFF有一个内部的合约，负责记录每个验证人错过的区块。 一旦该指标超过预定义的阈值，验证人的区块奖励将不会被转移到 FFF 进行分发，而是被其他更好的验证人共享。通过这种方式，运行不良的验证人会逐渐退出，因为它们的委托人将获得较少奖励或没有奖励。如果该数据仍然高于另一个较高的阈值级别，验证人将受到惩罚，并将传输回FFF，在FFF中，验证人的的抵押资产将被罚没一部分。

**参数管理**

有许多系统参数来控制 FFF 的行为，如罚息阈值和数量，转账费用等。所有这些参数将由 FFF 验证人通过提案投票过程确定。此过程将在 FFF 上进行，系统合约将通过通信来获取最新参数。

#### 激励

有两种主要的沟通方式：

1. 客户端操作，如转账和错误处理等。 这应该由事件请求者支付。
2. 系统同步，例如传递“退回资金”数据包（由于大多数Oracle中继失败造成的），或者用于验证的区块头，以及验证人集合更新。以上奖励由 FFF 系统合约支付。

如果某些中继器有更快的网络和更好的硬件，它们可以垄断所有的中继包，而不会给其他中继器留下任何收益。 因此，将有更少的参与者加入中继，这将鼓励集中化，但损害网络的效率和安全。 理想情况下，由于 FFF 验证人的分散化和动态重新选择，一个中继器不可能总是第一个传递每个消息。 但是为了避免进一步的垄断，奖励经济机制也是专门为尽量减少这种机会而设计的：

1. 对中继器的奖励将只分批次发放，而一次发放将覆盖多个成功的中继器包。
2. 一个中继器可以从批处理分发中获得的报酬与成功中继包的数量并不是成比例的。 相反，除了前几个数据包，在一个批次期间中继器传递传递数据包越多，它将获得的报酬越少。

### Oracle中继器

FFF的中继器使用 “Oracle”模型，也就是所谓的 “Oracle 中继器”。 每个FFF验证人都必须（只有验证集合中的验证人可以）运行 Oracle 中继器。 每个 Oracle 中继器都会观察 FFF状态的变化。 一旦它捕获到通信包，它将提交投票请求。在获得大于2/3投票支持更改之后，将执行跨链操作。

Oracle 中继器应该等待足够的区块来确认 FFF 的最终结果，然后才向 FFF 提交和投票通信包。

跨链费用将与正常的 FFF 区块奖励一起分配给 FFF 验证人。

此种 Oracle中继器依赖于所有验证人的支持。 由于跨链通信包的所有投票都记录在区块链上，因此评估 Oracle 中继器的性能并不难。将来可能会通过引入的另一种惩罚机制来限制表现最差的验证人的收益。


## 展望

对于FFF链的未来，很难做出一个定论，因为它从未停止进化。双链策略一方面为用户打开了灵活可扩展的编程之门，另一方面为用户保留了极速交易合转账的便利，但这只是FFF链发展的一个阶段。以下是一些值得关注的主题，以促进社区更好地获得更多的可用性和可扩展性：

1.为不同的业务用例添加不同的数字资产模型
2.实现将更多的数据源，特别是 3FEX 市场数据，从 3FEX传输到FFF
3.提供兼容以太坊及其未来升级，以及其他区块链的接口
4.改进钱包和区块链客户端的可用性




