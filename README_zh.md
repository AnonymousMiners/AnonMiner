
<p align="center">
  <a href="https://github.com/AnonymousMiners/AnonMiner">
    <img src="https://raw.github.com/AnonymousMiners/AnonMiner/master/AnonMiner.png" alt="Logo" width="600" height="104">
  </a>

  <h3 align="center">伪装 & 加密</h3>
  <p align="center">
   帮助您规避加密货币监管的程序
    <br />
    <a href="[https://github.com/AnonymousMiners/AnonMiner/issues](https://github.com/AnonymousMiners/AnonMiner/issues/new?assignees=&labels=unverified&template=bug_report.yml)">报告问题</a>
    ·
    <a href="[https://github.com/AnonymousMiners/AnonMiner/issues](https://github.com/AnonymousMiners/AnonMiner/issues/new?assignees=&labels=feature+request&template=feature_request.yml)">请求新功能</a>
    <br />
    <br />
      <a href="https://github.com/AnonymousMiners/AnonMiner/blob/main/README_zh.md">中文</a>
     ·  
     <a href="https://github.com/AnonymousMiners/AnonMiner">हिन्दी</a>
     ·
      <a href="https://github.com/AnonymousMiners/AnonMiner">Español</a>  
      ·
       <a href="https://github.com/AnonymousMiners/AnonMiner">français</a>  
      ·
     <a href="https://github.com/AnonymousMiners/AnonMiner">Русский язык</a>
     ·
     <a href="https://github.com/AnonymousMiners/AnonMiner">Deutsch</a>
     ·
      <a href="https://github.com/AnonymousMiners/AnonMiner">日本語</a>
     ·
      <a href="https://github.com/AnonymousMiners/AnonMiner">한국어</a>
  </p>
</p>


不同于市面上简单的TLS或AES隧道技术，**无名矿工**是一款**集反抽水、超频、主被控管理、主动对抗策略、伪装与加密、修改流量特征、调整流量比例模型**于一身的综合性自研**GPU挖矿程序**。

目前支持AE, Beam, CFX, CLO, Ergo, ETC, ETF, ETHO, ETHw, ETP, DAE, Neox, QKC, RVN。

>目前仅支持**Windows 64位**平台，其他平台将很快支持。

# Table of Contents
- [背景](#背景)
- [功能概览](#功能概览)
- [安装说明](#安装说明)
- [使用介绍](#使用介绍)
  - [常用功能](#常用功能)
  - [表格说明](#表格说明)
- [目录结构](#目录结构)
- [开发费用](#开发费用)
- [常见问题](#常见问题)
- [联系我们](#联系我们)
- [语言包](#语言包)
- [硬件要求](#硬件要求)
- [内核版本](#内核版本)
- [待实现功能](#待实现功能)
- [台面下的功能](#台面下的功能)
- [更新日志](#更新日志)

## 背景


随着越来越多的加密货币法规出台，毫无疑问，如果被确定为加密货币参与者，那将会严重增加矿工的成本。

无名矿工的诞生就是为了避免这种情况发生。

## 功能概览

- 支持**反抽水**模式
 - **伪装成正常的浏览网页流量**
   - 加密流量
     - 使用 AES 加密底层流量
      - 使用 HTTPS 伪装并加密表层流量
   - 修改流量特征
      - 自动调整数据包大小
     - 自动调整数据包发送时间间隔
      - 自动调整上传和下载流量的比例
 - **具有主动对抗策略**
   - 不同的伪装和加密策略
   - 随机网络噪音
   - 每个服务器都有独立的动态伪装页面
   - 自动跳过使用过的路线
   - 自动切换路由和更改加密配置
   - 自动从全球数百节点中筛选最优路线
- 简单的超频设置
- **支持主被控管理模式**
- 支持开机自动启动
- 支持惰性刷新
- 支持 IPv4 和 IPv6
- 自动保存设置
- **自动向被控分发及更新程序**
- **动态更新加密配置文件**
- 对最新匿名技术的不断追求
-  ...

## 安装说明

根据你的平台和处理器选择对应的安装包。

|平台                |CPU                          |[压缩包](https://github.com/AnonymousMiners/AnonMiner/releases) 后缀                         |
|------------------------|-----------------------------|-----------------------|
|Windows x64				|`Intel/AMD x86_64`            |win_amd64.zip           |




主机和客户端需要在**同一个局域网**中。

局域网中只需要一个主机。

>目前仅支持**Windows 64位**平台，其他平台将很快支持。


## 使用介绍

> **强烈推荐** 使用IPv6 以增强匿名性和稳定性。

#### 主控
![Host](https://raw.github.com/AnonymousMiners/AnonMiner/master/Images/Chinese.gif)
#### 被控
![enter image description here](https://raw.github.com/AnonymousMiners/AnonMiner/master/Images/Client.PNG)

> 如果翻译或表达有误，请告诉我们。 [联系我们](#联系我们)  or [报告问题](https://github.com/AnonymousMiners/AnonMiner/issues)

### 常用功能
|标签|说明  |
|--|--|
|**`返还开发费`**  |  劫持所有与钱包地址不匹配的连接（包括挖矿软件），并重定向到当前地址。 **默认处于关闭状态。** |
| **`开启局域网主控模式`** |**启用主被控管理模式**。这台机器将搜索并连接到同一局域网中运行着被控程序的所有机器。 |
| **`超频参数设置`** |本机的超频设置。如果“本机不参与挖矿”开启，本项将被禁用。 |
| **`被控通用设置`** | 被控的超频设置。将根据被控的显卡型号进行自动分配超频参数。|
| **`公告`** |官方公告。动态更新，敬请关注。 |



### 表格说明
自动切换到新的加密线路时，所有的记录（包括已接受、已拒绝和无效）将被清除。因此，请以矿池页面的记录为准。
> 将在下一个版本中修复。

|标签|说明  |
|--|--|
|**`内网IP`**  |  局域网内该机器的IP。（*代表本机）|
| **`拒绝`** |被矿池拒绝的计数。 程序将**自动尝试重新提交被矿池标记为拒绝的工作，以增加实际收益**。所以拒收率会比平时高一点。 |
| **`状态`** |具有已断开、已连接和运行中三种状态。 **开始挖矿时，需要等待一段时间（几十秒）**才能接收到矿池返回的数据并**显示在表格中**。 |
| **`汇报时间`** | 从机器接收到信息的最近时刻。|
| **`Auto Start`**|开机自动启动程序。|


## 目录结构
```
目录结构 
├── AnonMiner.exe
├── Config.json
├── AbandonedIP.json
├── README.md
├── /Miners/
│  ├── Various mining software
├── /Tools/
│  ├── Detection configuration tool
```

## 开发费用

基础开发费用为 **1.2%**。

当**返还开发费模式开启**时，开发费用如下：

|算法/币种|开发费用  |
|--|--|
|**ETHash coins**  |  0.2% |
|  **AE** | - 0.8% |
|**ERGO, NEOX, RVN**  |- 0.8% |
| **CFX** |- 1.8%  |
| **BEAM** | - 0.8% |


**注意**: 负数费用意味着您将获得比单独使用挖矿软件时，更多的算力。

>目前仅支持Nbminer，其他挖矿软件将很快支持。

## 常见问题

 1. 问题: 为什么软件界面出现乱码？
回答: 因为系统**缺少对应的文本包**，您需要从[语言包](#语言包)中下载并复制到**C:\Windows\Fonts**文件夹或系统盘的相似路径。

 2. 问题: 开始挖矿后，为什么表格中的数据没有刷新？
 回答: **因为需要等待一段时间（几十秒）**才能接收到矿池返回的数据并**显示在表格中**。

3. 问题: 为什么表中的数据不准确？
回答: 因为自动切换到新的加密线路时，所有的记录（包括已接受、已拒绝和无效）将被清除。所以，请以矿池页面的记录为准。
> 将在下一个版本中修复。

>期待您的提问。  [联系我们](#联系我们) 

## 联系我们

-   Email:  [AnonymousMiners@protonmail.com](mailto:AnonymousMiners@protonmail.com)
- [Telegram](https://t.me/AnonMinerNews)


## 语言包

>只有当软件界面出现乱码时，才需要安装语言包。

将其复制到**C:\Windows\Fonts** 文件夹或系统盘的相似路径。

- English, Español, français, Русский язык, Deutsch -- [times.ttf](https://github.com/AnonymousMiners/AnonMiner/blob/main/Fonts/times.ttf?raw=true)
- 中文 -- [simkai.ttf](https://github.com/AnonymousMiners/AnonMiner/blob/main/Fonts/simkai.ttf?raw=true)
- हिन्दी -- [Aparajita.ttf](https://github.com/AnonymousMiners/AnonMiner/blob/main/Fonts/Aparajita.ttf?raw=true)
- 日本語  -- [YuGothR.ttc](https://github.com/AnonymousMiners/AnonMiner/blob/main/Fonts/YuGothR.ttc?raw=true)
- 한국어 -- [Batang.ttc](https://github.com/AnonymousMiners/AnonMiner/blob/main/Fonts/Batang.ttc?raw=true)

> 如果有更好看的字体或翻译或表达错误，请告诉我们。 [联系我们](#联系我们)

## 硬件要求

> **仅对主控作出要求。**

最低配置:
* 2核以上的CPU
* 1.5GB 内存
* 8+ MBit/秒 **内网**速率
* 1+ MBit/秒 **公网**速率

推荐配置:

* 4核以上的CPU
* 4GB+ 内存
* 30+ MBit/秒 **内网**速率
* 10+ MBit/秒  **公网**速率

## 内核版本
| Miner | Version |
|--|--|
| NBMiner | 41.0 - 42.3 |

>目前仅支持Nbminer，其他挖矿软件将很快支持。

## 待实现功能

> 为了确保大家的安全，避免泄露所使用的伪装技术的细节，因此无法详细描述将要开发的功能。

> 如果您需要其他新功能，请在[问题页面](https://github.com/AnonymousMiners/AnonMiner/issues)中提出请求。

- 支持更多币种
- 支持更多的挖矿软件
- 更先进的伪装技术
- 更美观的界面
- 更准确的翻译
-  …

## 台面下的功能
请在 [项目文档](https://github.com/AnonymousMiners/AnonMiner/wiki) 中探索。

## 更新日志

v1.3 (2022-08-17)
- 重构主被控管理框架

v1.2 (2022-08-12)
- 新增自动向被控分发与更新程序
- 更强的伪装手段
- 增强稳定性
- 优化性能
- 新增从服务器下载最新适配挖矿软件功能
- 增加备用线路数目
- 增加主动对抗策略
- 修复偶发的被控失联问题

v1.1 (2022-08-01)
- 修复热更新配置闪退问题
- 增加多语言支持
- 支持被控开机自启
- 新增流量比例自动调节功能
- 内置检测工具
- 新增完整性检测

v1.0 (2022-07-19)
- 支持主被控管理模式
- 新增混淆方式
- 所有配置云端化
- 新增主动对抗策略

 …
 …
