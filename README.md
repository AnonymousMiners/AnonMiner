<p align="center">
  <a href="https://github.com/AnonymousMiners/AnonMiner">
    <img src="https://raw.github.com/AnonymousMiners/AnonMiner/master/AnonMiner.png" alt="Logo" width="600" height="104">
  </a>

  <h3 align="center">Camouflage & Encryption</h3>
  <p align="center">
    A program to help you evade cryptocurrency regulation
    <br />
  <a href="https://github.com/AnonymousMiners/AnonMiner/issues/new?assignees=&labels=unverified&template=bug_report.yml">Report bug</a>
    ·
    <a href="https://github.com/AnonymousMiners/AnonMiner/issues/new?assignees=&labels=feature+request&template=feature_request.yml">Request feature</a>
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

Anon Miner is a comprehensive **GPU mining program** that integrates **NoDevFee Mode, overclocking, Host-Client management, active countermeasures, camouflage and encryption, modification of mining traffic characteristics, and adjustment of download and upload traffic scale models.**

Anon Miner can **fully simulate all processes such as requests, handshakes, and connections for normal web browsing** by adding and adjusting various characteristics of mining traffic to achieve complete anonymity.

Currently supports all mainstream currencies and mining pools of NBMiner v41.0 - v42.3.  For details, check [Support Coins](#DevFee).

> For the corresponding address of the mining pool, please refer to [MiningPoolStats](https://miningpoolstats.stream/).

>Currently only the **Windows x64** platform is supported, other platforms will be supported very soon. [Releases](https://github.com/AnonymousMiners/AnonMiner/releases)

>Enter the notification channel to get the latest information. [Contact us](#Contact-us)

# Table of Contents
- [Background](#Background)
- [Feature Overview](#Feature-Overview)
- [Install](#Install)
- [Usage](#Usage)
  - [Common](#Common)
  - [Table](#Table)
- [Directory Description](#Directory-description)
- [Dev Fee](#DevFee)
- [FAQ](#FAQ)
- [Contact us](#Contact-us)
- [Language Pack](#Language-Pack)
- [Hardware Requirements](#Hardware-Requirements)
- [Support Miner List](#Support-Miner-List)
- [To Do List](#To-Do-List)
- [Features beneath the surface](#Features-beneath-the-surface)
- [Change Log](#Change-Log)

## Background

As more and more cryptocurrency regulations are rolled out, there is no doubt that it will seriously increase the cost of miners if identified as a cryptocurrency participant.

Anon Miner was born to avoid this from happening.

## Feature Overview

 - Support **No Dev Fee** mode
 - **Disguised as normal web traffic**
	 - Double encrypted traffic
	   - Encrypt underlying traffic with AES
	   - Use HTTPS to masquerade and encrypt surface traffic
	 - Modify Traffic Characteristics
	   - Automatically adjust packet size
	   - Automatically adjust the packet sending interval
	   - Automatically adjust the ratio of upload and download traffic
 - **Active confrontation strategy**
   -  Different masquerading and encryption strategies 
   - Random traffic noise
   - Each server has its own fake page and switches from time to time
   - Automatically skip used routes
   - Automatically switch routes and change encryption configuration
   - Automatically filter out the optimal route from hundreds of nodes around the world
- **Support Host-Client Mode**
- **Support automatic setting of Host&Client control firewall**
- **Support automatic prohibition of mining kernel networking to avoid leaking network information**
- **Automatically distribute and update programs to clients**
- **Dynamically update encryption configuration files**
- Easy overclocking setup
- Support boot auto-start
- Support lazy refresh
- Support IPv4 & IPv6
- Auto save settings
- The constant pursuit of the latest anonymous technology
-  ...

## Install

Select the corresponding installation package according to your platform and processor.

|Platform                |CPU                          |[Releases](https://github.com/AnonymousMiners/AnonMiner/releases) zip suffix                         |
|------------------------|-----------------------------|-----------------------|
|Windows x64				|`Intel/AMD x86_64`            |win_amd64.zip           |



The Host and Client need to be in the **same _Local Area Network_**.

Only one Host is required in a _Local Area Network_.

>Currently only the **Windows x64** platform is supported, other platforms will be supported very soon.

## Usage

> IPv6 is **strongly recommended** for enhanced anonymity and stability.

#### Host
![Host](https://raw.github.com/AnonymousMiners/AnonMiner/master/Images/English.gif)
#### Client
![enter image description here](https://raw.github.com/AnonymousMiners/AnonMiner/master/Images/Client.PNG)

> Please let me know if the translation or expression is wrong. [Contact us](#Contact-us)  or [Report bug](https://github.com/AnonymousMiners/AnonMiner/issues)

### Common
|Tag|Description  |
|--|--|
|**`Anti Dev Fee`**  |  Hijack all connections that do not match the wallet address (including mining software), and redirect to the current address.  **Off by default.** |
| **`Enable LAN Host mode`** |**Enable Host-Client mode**. This machine will search for and connect to all machines running the Client program in the same local area network. |
| **`Boost Config`** |Overclocking settings for this machine. This item will be disabled if "This machine does not participate in mining" is turned on. For the meaning of the parameters, please refer to [NBMiner](https://github.com/NebuTech/NBMiner#CMD-options). |
| `Independent Boost` |Overclocking settings for this machine. Set the overclocking parameters independently for each graphics card of this machine. When off, all graphics cards in this machine will use the same overclocking parameters. |
| **`Client General Settings`** | Overclocking settings for Clients. The overclocking parameters will be automatically assigned according to the Client's graphics card model.|
| **`Announcement`** |Official Announcement. Dynamic updates, please pay close attention. |



### Table
When switching to a new route automatically, all records (including Accepted, Rejected and Invalid) will be cleared. Therefore, please refer to the records on the mining pool page 
> Will be fixed in the next version.

|Tag|Description  |
|--|--|
|**`Intranet IP`**  |  The IP of the machine in the LAN. (* represents this machine)|
| **`Rejected`** |The program will **automatically attempt to resubmit the work marked as Rejected by the mining pool to increase the actual revenue**. So the rejection rate will be a bit higher than normal. |
| **`State`** |It has three states of Disconnected, Connected and Mining. **When you start mining, you need to wait for a while (tens of seconds)** to receive the data returned by the mining pool and **display in the Table**. |
| **`Report Time`** | The latest time the information was received from the machine.|
| **`Auto Start`**|Start the program automatically at startup.|


## Directory description
```
File tree 
├── AnonMiner.exe
├── Config.json
├── AbandonedIP.json
├── README.md
├── /Miners/
│  ├── Various mining software
├── /Tools/
│  ├── Detection configuration tool
```

## DevFee

> For the corresponding address of the mining pool, please refer to [MiningPoolStats](https://miningpoolstats.stream/).

When the **No Dev Fee mode is turned on**, the dev fee is as follows:

|Algorithm|Coins|Dev Fee  |
|--|--|--|
|**Ethash/Etchash**  |AKA, ATH, CLO, DAE, DBIX, EGEM, ELLA, ERGO, ESN, **ETC**, **ETF**, ETHO, **ETHW**, ETP, EXP, QKC|  0% |
|  **Kawpow** |ARL, HVQ, KAW, MEWC, NEOX, PRCO, **RVN**, SATO  |- 1% |
|  **Cuckoo Cycle** |**AE**, CTXC |- 1% |
|**Autolykos 2** | **ERGO** |- 1% |
| **Octopus** |CFX|- 2%  |
| **BeamHash** |Beam| - 1% |

**Note**: Negative rates mean you'll get extra income than using the mining software alone.

**When NoDevFee mode is turned off**, the dev fee is 1%.

>Currently only supported Nbminer,  other mining software will be supported soon.

## FAQ

1. Q: Why does the software interface appear garbled?
A: Because the system **lacks the corresponding text package**, you can download it from [Language Pack](#Language-Pack)  and copy it to **C:\Windows\Fonts** folder or a similar path to the system disk.

2. Q: After starting, why is the data not refreshed?
A: When you start mining, you need to wait for a while (tens of seconds) to receive the data returned by the mining pool and **display in the Table**. 

3. Q: Why is the data in the table inaccurate?
A: When switching to a new route automatically, all records (including Accepted, Rejected and Invalid) will be cleared. Therefore, please refer to the mining pool page for records.
> Will be fixed in the next version.

>Looking forward to your questions.  [Contact us](#Contact-us) 

## Contact us

-   Email:  [AnonymousMiners@protonmail.com](mailto:AnonymousMiners@protonmail.com)
- Telegram
  - [**Notification channel**](https://t.me/AnonMinerNews)
  - [English community](https://t.me/AnonMinerGlobal)
  - [中文社区](https://t.me/AnonMinerZh)
  - [हिंदी समुदाय](https://t.me/AnonMinerHindi)


## Language Pack

>Only when garbled characters appear in the software interface, you need to install the language pack.

Copy it to **C:\Windows\Fonts** folder or a similar path to the system disk.

- English, Español, français, Русский язык, Deutsch -- [times.ttf](https://github.com/AnonymousMiners/AnonMiner/blob/main/Fonts/times.ttf?raw=true)
- 中文 -- [simkai.ttf](https://github.com/AnonymousMiners/AnonMiner/blob/main/Fonts/simkai.ttf?raw=true)
- हिन्दी -- [Aparajita.ttf](https://github.com/AnonymousMiners/AnonMiner/blob/main/Fonts/Aparajita.ttf?raw=true)
- 日本語  -- [YuGothR.ttc](https://github.com/AnonymousMiners/AnonMiner/blob/main/Fonts/YuGothR.ttc?raw=true)
- 한국어 -- [Batang.ttc](https://github.com/AnonymousMiners/AnonMiner/blob/main/Fonts/Batang.ttc?raw=true)

> Please let us know if there is a better looking font or a translation or expression error.  [Contact us](#Contact-us)

## Hardware Requirements

> **Only required for Host.** 

Minimum:
* CPU with 2+ cores
* 1.5GB RAM
* 8 MBit/sec **Intranet** service
* 1 MBit/sec **Internet** service

Recommended:

* Fast CPU with 4+ cores
* 4GB+ RAM
* 30+ MBit/sec **Intranet** service
* 10+ MBit/sec **Internet** service

## Support Miner List

| Miner | Version |
|--|--|
| NBMiner | 41.0 - 42.3 |

>Currently only supported Nbminer,  other mining software will be supported soon.

## To Do List

> In order to ensure everyone's safety and avoid leaking the details of the camouflage techniques used, it is impossible to describe the features that will be developed in detail.

> If you need additional new features, please make a request in the [issue](https://github.com/AnonymousMiners/AnonMiner/issues).

- Support more Coins
- Support more Mining software
- More advanced camouflage technology
- Better looking interface
- More accurate translation
-  …

## Features beneath the surface
Explore the [documentation](https://github.com/AnonymousMiners/AnonMiner/wiki) for this project.

## Change Log
v1.3.2 (2022-10-02)

- Improve display logic.
- Increase overclocking parameters.
   -  Temperature upper bound.
   -  Restart temperature after reaching the upper bound.
   
v1.3.1 (2022-09-22)

- Fix local display bug
- Fix some translation errors

v1.3 (2022-08-17)
- Replacing the Host-Client Architecture

v1.2 (2022-08-12)
- Automatic distribution program
- Stronger camouflage encryption
- Enhanced stability
- Enhanced performance
- Added the function of downloading miners from the server
- Increase the number of alternate routes
- Increase active countermeasures
- Fixed occasional disconnection of Client

v1.1 (2022-08-01)
- Fix hot update configuration flashback
- Add multi-language support
- Support Client boot automatically
- Add the function of automatically adjusting the flow ratio
- Built-in detection configuration tool
- Add program completeness detection function

v1.0 (2022-07-19)
- Support Host-Client mode
- Add obfuscation
- All configurations are cloud-based now
- Increase active countermeasures

…
…
