| FATIP | Title                      | Status   | Category | Author                                         | Created    |
| ----- | -------------------------- | -------- | -------- | ---------------------------------------------- | ---------- |
| 111   | Universal Oracle Spec      | WIP      | Core     | Sergey Bushnyak \<s.bushnyak@kelecorix.com\>   | 2020-03-20 |

# Universal Oracle Specification

## Summary

This standard identifies common formats and features for building universal decentralized oracle systems on FAT. The Oracle system Allows to create smart-contracts with connectivity to real-time data feeds.

## Motivation

Modern decentralized applications (dApps) require means to access real-world data in an organized and reliable way. Since this data exists outside of blockchain we need to establish a trustworthy workflow that allows us to collect this data on chain and verify its correctness. In the same time smart-contract developers should have the ability to get real-time data from trusted oracle providers within their code without a need to spend time on developing custom solutions.

Some examples of potential use:
- An oracle that collects weather data could allow an earthquake insurance contract. Users purchase coverage from the smart contract, which pays out when there’s a sufficiently severe earthquake in their area.
- An oracle collects data from iot soil sensors in specific area and store intraday difference can release support funds for farmers when soil moisture stays low for defined period
- A combination of standalone oracles can be used to provide consensus, where only results published by a majority of the oracles are considered valid, ie. PegNet
- An oracle that provides FCT/USD prices could allow users to deposit funds that are immediately converted to some on-chain asset and represented as fiat
- Trusted parties could expose data API’s on-chain specific for theirs use case
- <add more compelling examples>

In centralized or semi-centralized oracles, a trusted party or low number of trusted partners simply attests to the validity of the data using cryptographic signature(s). However, as implied, the data is only as trustworthy as the data provider, also known as “The Oracle Problem”. This challenge is often regarded as one of the great limitations of blockchain technology’s applicability in traditional domains.

In a decentralized oracle system, different on-chain tokenomics or (less often) governance mechanics are used to mediate trust. In some systems, these economic incentives are similar to the “encouragement and punishment”  mechanisms seen in Proof-of-Stake systems which find quite good.
<there is a very close coupling to gas mechanics FAT-108 and being an oracle should be harder than just verifying to provide trust, looking for additional fees?
PegNet uses a combination of PoW(miners calculate hard hash and push data) and PoS(stakers that have a lot of funds just push data) providers and average settlement on majority of data. ChainLink better at this stuff as provider, needs more investigation, as potentially with this contract format users can build the very same PegNet but in smart-contracts >


## Specification

### Initiate contract

### Getting values

Raw JSON value when getting data
```
{
  "rows": [{
      "id": "0",
      "owner": "eq-monitor",
      "value": 56800,
      "median": 56863,
      "timestamp": "1564096083"
    }
  ],
  "more": true
}
```

### Updating values
### Connecting update server

## Implementation

## Copyright
Copyright and related rights waived via CC0.
