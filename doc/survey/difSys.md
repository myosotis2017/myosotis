## 其他系统调研

### 一. vnpy
> vnpy是现在比较成熟的cs框架下得python为基础的应用，由经验的交易员开发，因此其开发的功能模块和设计的思路有很强的参考价值。

分析其系统的构成对系统的设计具有指导意义。

#### 系统架构

![ALgoFramework系统架构](ALgoFramework.png)

通过分析其系统架构：

1. 系统边界，从底层来说主要是从哪里获取数据，经过系统或者人机交互之后数据或者形成的产品交给谁，另外就是数据的持久化，或者用户的应用数据的存储。
2. 整个系统也是分成这几个部分：从别的api中获取数据，进行应用的数据处理，形成产品或指令给交易的api，业务的核心是在数据处理层。
3. 应用逻辑层：各种引擎（定价引擎）
