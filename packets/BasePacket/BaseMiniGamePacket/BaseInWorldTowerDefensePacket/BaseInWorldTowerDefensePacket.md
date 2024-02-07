
| Offset | Size | Name | Confidence | Verification | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| 4 | 4 | op code 2 | H | D | `54` (`0x36`). Distinguishes subclasses/children of `BaseInWorldTowerDefensePacket` from other children. |
| 8 | 4 | match ID | L | D | Used. |
| 12 | 4 |  | H | D | Unused. Always `-1` (`0xffffffff`). |
| 16 | 4 |  | H | D | Unused. Always `-1` (`0xffffffff`). |
| 20 | 4 | op code 3 | H | D | Oddly, Republic Defender packets ignore the unused space above and have a custom field for the third op code. |
| 24 | 4 |  | L | D | Seemingly always `0`. |
## InWorldTowerDefenseDeckPacket

| Offset | Size | Name | Confidence | Verification | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| 20 | 4 | op code 3 | H | D | `2` (`0x2`). |
| 24 | ? | tower types | L | D | `SoeUtil::Array<DeckSlot, 0, 1>` type. |
## InWorldTowerDefenseGameStatePacket

## InWorldTowerDefenseInventoryPacket

## InWorldTowerDefenseNotifyPacket

## InWorldTowerDefenseOptionPacket

## InWorldTowerDefensePacketTowerTransaction

## InWorldTowerDefenseUpdateDeckPacket

| Offset | Size | Name | Confidence | Verification | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| 20 | 4 | op code 3 | H | D | `7` (`0x7`). |
| 24 | 4 |  | L | D | Seemingly always `0`. |
| 28 | 4 |  | L | D | Seemingly always `0`. |
| 32 | 1 |  | L | D | Seemingly always `1`. Used as boolean flag. Referenced in `FUN_00a8e840`. (`(int)this + 0x24` accounts for 4-byte vtable in `BasePacket`.) |
| 33 | 1 |  | L | D | Seemingly always `0`. Used as boolean flag. Referenced in `FUN_00a8e840`. (`(int)this + 0x25` accounts for 4-byte vtable in `BasePacket`.) |
## InWorldTowerDefenseWavesPacket
| Offset | Size | Name | Confidence | Verification | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| 20 | 4 | op code 3 | H | D | `3` (`0x3`). |
| 24 | 4 |  | L | D | Seemingly always `0`. |
| 28 | 21 | wave list | L | D | `HashList<InWorldTowerDefenseWave, 16, -1>` type. |
| 32 | 21 | enemy list | L | D | `HashList<InWorldTowerDefenseEnemyEntry, 16, -1>` type. |
| 33 | 32 (?) |  | L | D | `Array<int, 8, 1>` type. |
