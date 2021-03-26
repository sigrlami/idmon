| FATIP | Title                      | Status   | Category | Author                                         | Created    |
| ----- | -------------------------- | -------- | -------- | ---------------------------------------------- | ---------- |
| 111   | Universal Oracle Spec      | WIP      | Core     | Sergey Bushnyak \<s.bushnyak@kelecorix.com\>   | 2020-03-20 |

# Universal Oracle Specification

## Summary

This standard identifies common formats and features for building universal decentralized oracle systems on FAT. The Oracle system Allows to create smart-contracts with connectivity to real-time data feeds.

## Motivation

Modern decentralized applications (dApps) require means to access real-world data in organized and reliable way. Since this data exists outside of blockchain we need to establish trustworthy workflow that allow to collect this data on chain and verify its correctness.

Some examples of potential use:

- An oracle that collects weather data could allow an earthquake insurance contract. Users purchase coverage from the smart contract, which pays out when there’s a sufficiently severe earthquake in their area.
- An oracle collects data from iot soil sensors in specific area and store intra-day difference can release support funds for farmers when soil moisture stays low for defined period
- A combination of standalone oracles can be used to provide consensus, where only results published by a majority of the oracles are considered valid, ie. PegNet
- An oracle that provides FCT/USD prices could allow users to deposit funds that are immediately converted to some on-chain asset and represented as fiat
- Trusted parties could expose data API’s on-chain specific for theirs use case

## Specification

## Implementation

## Copyright
Copyright and related rights waived via CC0.
