---
eip: XXXX
title: Data Gas Increase
description: Increase both the data gas target and limit.
author: Dankrad Feist (@dankrad), Ansgar Dietrichs (@adietrichs)
discussions-to: TBD
status: Draft
type: Standards Track
category: Core
created: 2023-06-01
requires: 4844
---

## Abstract

TBD

## Motivation

TBD

## Specification

| Constant | Value |
| - | - |
| `MAX_DATA_GAS_PER_BLOCK` | `2**20` |
| `TARGET_DATA_GAS_PER_BLOCK` | `2**19` |
| `DATA_GASPRICE_UPDATE_FRACTION` | `4451303` |

## Rationale

The parameter `DATA_GASPRICE_UPDATE_FRACTION` is updated to keep targeting a maximum change rate of `e(TARGET_DATA_GAS_PER_BLOCK / DATA_GASPRICE_UPDATE_FRACTION) ≈ 1.125` per block.

## Backwards Compatibility

TBD

## Test Cases

TBD

## Security Considerations

TBD

## Copyright

Copyright and related rights waived via [CC0](../LICENSE.md).