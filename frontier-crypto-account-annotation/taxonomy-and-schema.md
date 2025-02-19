# 🏦 Crypto Account Annotation - Taxonomy and Schema


## 🌟 Introduction

**Account annotation** is critical for enhancing transparency and understanding within blockchain ecosystems. This process involves assigning metadata to blockchain addresses, providing insights into the identities, purposes, and behaviors associated with them. Account annotations are valuable across a range of applications, including:

- **🛡️ AML (Anti-Money Laundering) Management**: Account annotations help identify and monitor addresses involved in high-risk or illicit activities, such as money laundering or fraud. This enhances compliance with regulatory requirements and supports law enforcement investigations.
- **📈 On-Chain Marketing and Trend Analysis**: By understanding user behavior and activity patterns, companies can conduct targeted marketing and analyze trends in user engagement, token usage, and DeFi participation. Annotated data allows for in-depth insights into audience segments and market trends.
- **⚠️ Risk Management**: Financial institutions and crypto platforms leverage account annotations to assess risks associated with specific addresses, such as identifying potentially malicious or high-risk actors. This supports a proactive approach to security and compliance.
- **🌐 Reputation and Identity Systems**: Account annotations contribute to building reputation scores and trust networks by marking addresses with a history of positive or negative actions.

The taxonomy and schema provided here are designed to standardize data across these use cases, facilitating reliable, reusable account data across the industry.

> **Alternative Names**: Account annotation is also known as **address labeling**, **entity classification**, and **wallet tagging** within blockchain communities. Each term refers to the practice of categorizing blockchain addresses with meaningful metadata.


### 🤝 Call for Contributions
---
Codatta invites collaboration and contributions from research institutions, industry experts, and community members. If your organization or team is interested in enhancing these standards or proposing new use cases, please reach out. We welcome joint efforts to expand the taxonomy and address evolving industry needs.

For inquiries, contributions, or to propose a collaboration, please contact us at **[dev-opensource@codatta.io](mailto:dev-opensource@codatta.io)**.

## 📑 Source

The **Source** value provides information about how the given data entry was collected. We define five source values in the data model:

- **🌍 Ground Truth**: This method relies on conducting real-life transactions on-chain to identify blockchain addresses belonging to a specific entity. For example, depositing a small amount of ETH to identify addresses owned by a particular exchange.
- **🔍 Heuristic**: Clusters addresses using models based on publicly available information, such as transaction patterns. Examples include the Commonspend heuristic for UTXO chains.
- **🤖 Machine Learning**: Utilizes machine learning algorithms with on/off-chain data to create address clustering models.
- **📚 Research**: Relies on thorough research over publicly available information, especially useful during significant events in the space.
- **📥 External**: Gathers metadata from other open sources, like Etherscan.

## 🌐 Chain

The **Chain** indicates the blockchain or network where the address resides. The protocol has a fixed list of values defined in the data model, with flexibility to add new chains to accommodate metadata from emerging networks.

## 🏢 Entity

The **Entity** represents the owner of a given address, often at an organizational level. For instance, various Uniswap addresses for different purposes share the same entity name, "Uniswap." New entity values can be added as required by emerging networks.


## Category

The 'Category' value provides the additional information about the purpose or the sector of the address. For example, weather the address belongs to a centralised exchange, or whether the address is used by a DeFi project.

The protocol has a fixed list of values defined at the data model (as shown below) but new category values can be added to accommodate metadata from new blockchain networks.

|Category|Description|
|--------|-----------|
|Cold Storage|An offline wallet used to securely store large amounts of cryptocurrency for extended periods of time.|
|Hot wallet|An online wallet that offers easy and quick access to cryptocurrency funds for everyday use.|
|Deprecated|A smart contract that is no longer in use and has been deprecated by the protocol or development team.|
|Multisig|An address that requires approval from multiple parties to access cryptocurrency funds, providing an additional layer of security. Commonly used by exchanges and institutional investors.|
|Vault|A smart contract-based system that automatically invests cryptocurrency funds to generate yield for users, commonly used in decentralized finance (DeFi) applications and managed by the protocol or community.|
|Vault User|An address that interacted with a smart contract-based system that automatically invests cryptocurrency funds to generate yield for users, commonly used in decentralized finance (DeFi) applications and managed by the protocol or community.|
|Vulnerable|An address whose private keys have been compromised or are publicly available, exposing it to the risk of unauthorized access or theft.|
|Smart Contract|An address used by developers or teams to deploy smart contracts on a blockchain for decentralized applications or other projects.|
|NFT|An address controlled by an NFT marketplace that facilitates the buying, selling, or trading of non-fungible tokens.|
|DEX|An address or wallet used in decentralized exchanges to facilitate peer-to-peer trading of cryptocurrencies without a central authority.|
|DEX User|An address that interacted with a smart contract for a decentralized exchange used to facilitate peer-to-peer trading of cryptocurrencies without a central authority.|
|CEX|A centralized exchange (CEX) that allows users to trade cryptocurrencies in exchange for fiat or other cryptocurrencies.|
|ATM|Related to a cryptocurrency ATM that allows users to buy or sell cryptocurrencies using cash or debit/credit cards.|
|Auction|Related to an auction that can be held by a variety of entities, including law enforcement agencies (LEA).|
|Gambling|Related to a gambling website that allows users to place bets on various games using cryptocurrencies.|
|Gaming|Related to a gaming platform or game that allows users to buy, sell or trade digital assets or in-game items.|
|LE (Law Enforcement)|An address or wallet certified to belong to a law enforcement agency (LE).|
|Lending|Related to lending or borrowing activities in the crypto space, such as those belonging to lending platforms or peer-to-peer lending services.|
|Lending User|An address that interacted with a smart contract belonging to lending platforms or peer-to-peer lending services.|
|Merchant|Addresses or wallets that are associated with merchants who accept payment in cryptocurrencies.|
|Mixer|Addresses or wallets that are associated with crypto mixers or tumblers, which are services that mix multiple transactions together in order to obfuscate the origin of the funds.|
|Payment Processor|Related to a business that facilitates transactions between buyers and sellers using cryptocurrency as payment.|
|Business or Services, Other|Related to a business or service that operates within the crypto ecosystem but does not fit into any of the other categories.|
|Token Team|An address or wallet that is controlled by the team responsible for creating and maintaining a particular cryptocurrency token.|
|Weapons|An address or wallet that is involved in the sale or exchange of weapons using cryptocurrency.|
|Marketplace Aggregator|Related to a business or service that consolidates data from multiple decentralized exchanges or NFT markets in order to provide users with a comprehensive view of the market.|
|L2|An address or wallet associated with a layer 2 scaling solution built on top of the Ethereum network.|
|Insurance|Related to A business or service that provides insurance coverage for cryptocurrency assets stored on the blockchain.|
|Asset Management|Related to A business or service that manages cryptocurrency assets on behalf of clients.|
|Streaming|Related to A business or service that provides streaming media content using cryptocurrency payments.|
|Infra|Related to A business or service that provides infrastructure services to support the operation of blockchain networks.|
|Oracle|Related to A service that provides off-chain data to smart contracts. Oracles allow smart contracts to interact with external data sources, making them more versatile and useful.|
|DAO|Related to A DAO is an organization that is run by rules encoded as computer programs called smart contracts.|
|Yield|Related to a yield service allows users to earn interest on their cryptocurrency deposits.|
|Wallet|A wallet is a software or hardware device used to store cryptocurrency private keys and sign transactions.|
|Fund|A fund is an entity that pools capital from multiple investors and uses it to invest in a variety of assets, including cryptocurrencies.|
|Derivatives|A derivatives entity is an organization that specializes in trading cryptocurrency derivatives, such as futures, options, and swaps.|
|E-Commerce|An e-commerce entity is an organization that uses cryptocurrency as a payment method for goods and services.|
|Identity|An identity entity is an organization that provides on-chain identity-related products, such as decentralized identifiers (DIDs) and verifiable credentials.|
|Mining Pool|An organization that brings together multiple miners to collectively mine cryptocurrency.|
|Liquid Staking|Companies that allow users to stake their PoS tokens and receive liquid staking derivatives in exchange.|
|Payments|Associated with companies providing on-chain payment processing services, allowing users to send and receive cryptocurrency payments on the blockchain.|
|Sidechain|Associated with sidechain solutions built on top of the Ethereum blockchain, allowing developers to deploy decentralized applications with increased throughput and scalability.|
|Router|Associated with router services that allow users to swap tokens across multiple liquidity pools.|
|Coin Swapper|Associated with services that allow users to swap one cryptocurrency for another without requiring users to deposit funds into the service wallet first.|
|Sport|Associated with sport-related products or services, including fantasy sports, sports betting, and collectibles.|
|Privacy (not Mixer)|Associated with products or services that provide privacy solutions on the blockchain.|
|Validator|Associated with validators that help secure Proof-of-Stake (PoS) blockchain networks.|
|Charity|Controlled by an organization that accepts crypto donations for charitable causes|
|Donation|Controlled by an organization that accepts crypto donations for any purpose|
|Deployer|Addresses that has been used to deploy smart contracts|
|Company Funds|Addresses managed by companies, projects or foundations, which are usually used for treasury management, paying salaries or other expenses|
|Eth 2 staker|Addresses that have staked Ether at the Ethereum 2.0 Beacon Chain to help secure the network and earn rewards|
|Yield Farming|Addresses used for yield farming strategies where users can deposit cryptocurrencies to earn rewards and/or fees on a decentralized platform|
|Yield Aggregator User|An address that interacted with a smart contract used for yield farming strategies where users can deposit cryptocurrencies to earn rewards and/or fees on a decentralized platform|
|ICO|Addresses used to receive funds during an initial coin offering (ICO) or other crowdfunding mechanisms|
|Stablecoin|Addresses used for stablecoin projects, including centralized and decentralized stablecoins|
|Staking|Addresses used for staking, where users can lock up their cryptocurrency to help secure a network and earn rewards|
|Token Sale|Addresses used during a token sale where users can buy tokens at an initial price, including initial coin offerings (ICO) and initial dex offerings (IDO)|
|Defi|Addresses used for decentralized finance (DeFi) projects, including decentralized exchanges, yield farming, lending, and more|
|Defi User|An address that interacted with a smart contract used for decentralized finance (DeFi) projects, including decentralized exchanges, yield farming, lending, and more|
|Advertising|Addresses used for advertising-related activities in the crypto environment.|
|Energy|Addresses used by entities that are bringing energy-related products into the blockchain.|
|FIAT|Addresses controlled by businesses that allow customers to trade fiat currencies.|
|KYC|Used for exchanges or other service that require customers to provide a valid ID document to trade fiat-to-crypto or crypto-to-crypto.|
|NO KYC|Used for exchanges or other service that do not require customers to provide a valid ID document to trade fiat-to-crypto or crypto-to-crypto.|
|Darknet|Addresses belonging to services hosted on the dark web, or being involved in dark web transactions.|
|Money Laundering|Addresses certified belonging to money laundering activities.|
|Malware|Addresses belonging to malware campaigns.|
|Ransom|Addresses that have been identified as being involved in ransomware attacks.|
|Scam|Addresses that have been identified as being involved in fraudulent activities or scams.|
|Terrorism|Addresses that have been identified as being involved in financing terrorism.|
|Theft|Addresses that have been identified as being involved in theft or hacking of cryptocurrencies.|
|Sanctioned|Addresses that have been sanctioned by some governments in the world.|
|Phishing|Addresses related to phishing scams|
|Ponzi|Addresses related to Ponzi schemes|
|Spam|Addresses related to spamming|
|Fake KYC|Addresses related to fake KYC procedures|
|Malicious Mining Activities|Addresses used for mining cryptocurrencies with malware or botnets|
|Financial Crime, Other|Addresses related to financial crimes such as money laundering, fraud, and tax evasion|
|Cybercrime|Addresses related to cybercrimes such as hacking, data theft, and ransomware|
|Honeypot|Addresses related to fake tokens or ICOs that are designed to scam investors or traders|
|Black Mail Activities|Addresses that threaten to reveal sensitive information or personal data in exchange for ransom payments|
|Constrained by Service|Addresses that have been restricted or blocked from using centralized or decentralized exchanges due to suspicious activities or high risk status|
|High Risk, Other|Addresses that are associated with suspicious, fraudulent, or illegal activities that are not covered by other categories|
|Dapp, Other|Addresses used by decentralized applications (dApps) to interact with smart contracts and blockchain networks|
|Bridging|Addresses used by platforms or projects that provide interoperability solutions to connect different blockchain networks|
|Bridge User|An address that interacted with a smart contract used by platforms or projects that provide interoperability solutions to connect different blockchain networks|
|Multichain|Addresses used by platforms or projects that enable communication and transfer of assets between multiple blockchain networks|
|Factory Contract|Smart contracts used to create and deploy multiple instances of other smart contracts|
|Fraud Proof|Smart contracts used to prove fraudulent activities or invalid state transitions on layer 2 protocols|
|Genesis|Genesis addresses used to mint/burn|
|MEV Bot|Addresses used by MEV bots for transaction extraction and prioritization|
|Proxy|Contract that acts as a proxy to another contract and is used to upgrade the logic of the target contract without changing its address|
|Exchange|Addresses used by centralized or decentralized exchanges to interact with smart contracts and blockchain networks|

## 🛠 Schema

The schema we use for organizing account annotation is based on the initial version proposed by [Microscope Protocol's blockchain metadata schema](https://github.com/microscopexyz/chainmetareader/blob/main/doc/taxonomy.md), which has served as a foundational framework for standardizing account annotation aggregation across providers. We attribute the original schema design to [Microscope Protocol](https://microscopeprotocol.xyz/), recognizing their efforts to establish industry standards (check detail in the [Acknowledgment](#-acknowledgment) section).

> **Note**: While we adopt this schema as an industry-wide best practice, future iterations may include updates and modifications to meet evolving requirements and enhance functionality.

```json
{
  "address": "string",
  "name": "string",
  "source": {
    "type": "string",
    "enum": ["Ground Truth", "Heuristic", "Machine Learning", "Research", "External"]
  },
  "chain": "string",
  "entity": "string",
  "category": {
    "type": "string",
    "enum": [
      "Cold Storage",
      "Hot wallet",
      "Deprecated",
      "Multisig",
      "Vault",
      "Vault User",
      "Vulnerable",
      "Smart Contract",
      "NFT",
      "DEX",
      "DEX User",
      "CEX",
      "ATM",
      "Auction",
      "Gambling",
      "Gaming",
      "LE (Law Enforcement)",
      "Lending",
      "Lending User",
      "Merchant",
      "Mixer",
      "Payment Processor",
      "Business or Services, Other",
      "Token Team",
      "Weapons",
      "Marketplace Aggregator",
      "L2",
      "Insurance",
      "Asset Management",
      "Streaming",
      "Infra",
      "Oracle",
      "DAO",
      "Yield",
      "Wallet",
      "Fund",
      "Derivatives",
      "E-Commerce",
      "Identity",
      "Mining Pool",
      "Liquid Staking",
      "Payments",
      "Sidechain",
      "Router",
      "Coin Swapper",
      "Sport",
      "Privacy (not Mixer)",
      "Validator",
      "Charity",
      "Donation",
      "Deployer",
      "Company Funds",
      "Eth 2 staker",
      "Yield Farming",
      "Yield Aggregator User",
      "ICO",
      "Stablecoin",
      "Staking",
      "Token Sale",
      "Defi",
      "Defi User",
      "Advertising",
      "Energy",
      "FIAT",
      "KYC",
      "NO KYC",
      "Darknet",
      "Money Laundering",
      "Malware",
      "Ransom",
      "Scam",
      "Terrorism",
      "Theft",
      "Sanctioned",
      "Phishing",
      "Ponzi",
      "Spam",
      "Fake KYC",
      "Malicious Mining Activities",
      "Financial Crime, Other",
      "Cybercrime",
      "Honeypot",
      "Black Mail Activities",
      "Constrained by Service",
      "High Risk, Other",
      "Dapp, Other",
      "Bridging",
      "Bridge User",
      "Multichain",
      "Factory Contract",
      "Fraud Proof",
      "Genesis",
      "MEV Bot",
      "Proxy",
      "Exchange"
    ]
  },
  "submit_on": {
    "type": "string",
    "format": "date-time",
    "description": "The ISO timestamp of when the data was sourced, in the format YYYY-MM-DD HH:MM:SS"
  },
  "description": {
    "type": "string",
    "description": "A human-readable description of the address or entity"
  },
  "evidence_uri": {
    "type": "string",
    "format": "uri",
    "description": "The multimedia link of the evidence"
  },
  "submit_by": {
    "type": "string",
    "description": "The code of the operator, in the format 'operator:workflow', e.g., 'coinbase:workflowA' or 'circle:laberB'"
  }
}
```
This schema defines the JSON structure for annotating crypto accounts/addresses, reflecting the implementation and best practices used at Codatta for sourcing and categorizing data in this frontier. Contributors should follow this schema to ensure consistency and compatibility. 

> **Note**: While this schema represents Codatta’s current practices, modifications may occur during actual implementation due to engineering and product considerations.

## 📜 Acknowledgment
We gratefully acknowledge the contributions of the Microscope Protocol for building a foundational framework that supports standardization in the industry. Their pioneering work has provided a significant foundation for the schema and taxonomy used here, advancing the practice of account annotation and making industry-wide standardization achievable. You can view their original taxonomy documentation at [Microscope Protocol - Taxonomy Documentation](https://github.com/microscopexyz/chainmetareader/blob/main/doc/taxonomy.md).