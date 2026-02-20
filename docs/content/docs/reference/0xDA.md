---
title: 0xDA - Info Response
weight: 26
---

This packet is exclusively emitted by the Door Lock in response to the [`0x5A`](../0x5A) packet.

## Specification

| Byte | Description | Values |
| ---- | ----------- | ------ |
| 1    | Packet ID   | `0xDA` |
| 2    | Unknown     | `0x02` |
| 3    | Unknown     | `0x00` |
| 4    | Unknown     | `0x00` |
| 5    | Unknown     | `0x07` |
| 6    | Unknown     | `0x02` |
| 7    | Unknown     | `0x00` |

## Examples

```
FF 48 07 DA 02 00 00 07 02 00 EC
```
