
| Offset | Size | Name | Confidence | Verification | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| 8 | 4 | match ID | L | D | Used. |
| 12 | 4 |  | H | D | Unused. Always `-1` (`0xffffffff`). |
| 16 | 4 |  | H | D | Unused. Always `-1` (`0xffffffff`). |
| 20 | 4 | op code 3 | H | D | Oddly, Republic Defender packets ignore the unused space above and have a custom field for the third op code. |
| 24 | 4 |  | L | D | Seemingly always `0`. |
## InWorldTowerDefenseDeckPacket

## InWorldTowerDefenseGameStatePacket

## InWorldTowerDefenseInventoryPacket

## InWorldTowerDefenseNotifyPacket

## InWorldTowerDefenseOptionPacket

## InWorldTowerDefensePacketTowerTransaction

## InWorldTowerDefenseUpdateDeckPacket

## InWorldTowerDefenseWavesPacket