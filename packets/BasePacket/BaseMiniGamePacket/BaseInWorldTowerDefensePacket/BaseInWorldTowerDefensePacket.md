| Offset | Size | Name | Confidence | Verification | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| 4 | 4 | op code 2 | H | D | `54` (`0x36`). |
| 8 | 4 | match ID | L | D | Used. |
| 12 | 4 |  | H | D | Unused. Always `-1` (`0xffffffff`). |
| 16 | 4 |  | H | D | Unused. Always `-1` (`0xffffffff`). |
| 20 | 4 | op code 3 | H | D | Oddly, Republic Defender packets ignore the unused space above and have a custom field for the third op code. |
| 24 | 4 |  | L | D | Seemingly always `0`. |
## InWorldTowerDefenseDeckPacket
| Offset | Size | Name | Confidence | Verification | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| 20 | 4 | op code 3 | H | D | `2` (`0x2`). |
| 24 | 4 |  | L | D | Seemingly always `0`. |
| 28 | ? | power-ups | L | D | `SoeUtil::Array<DeckSlot, 0, 1>` type.  |
## InWorldTowerDefenseGameStatePacket
| Offset | Size | Name | Confidence | Verification | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| 20 | 4 | op code 3 | H | D | `4` (`0x4`). |
| 24 | 4 |  | L | D | Seemingly always `0`. |
| 28 | 4 |  | L | D | Initialized to `0`. Updated in `FUN_00a8bff0`. |
| 32 | 4 |  | L | D | Initialized to `0`. Updated in `FUN_00a8bff0`. |
| 36 | 4 |  | L | D | Initialized to `0`. Updated in `FUN_00a8bff0`. |
| 40 | 4 |  | L | D | Initialized to `0`. Updated in `FUN_00a8bff0`. |
| 44 | 4 |  | L | D | Initialized to `0`. Updated in `FUN_00a8bff0`. |
| 48 | 4 |  | L | D | Initialized to `0`. Updated in `FUN_00a8bff0`. |
## InWorldTowerDefenseInventoryPacket
| Offset | Size | Name | Confidence | Verification | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| 20 | 4 | op code 3 | H | D | `1` (`0x1`). |
| 24 | 4 |  | L | D | Seemingly always `0`. |
| 28 | 45 | towers | L | D | `HashList<InWorldTowerDefenseTower, 64, -1>` type. |
| 61 | 36 | special power-ups | L | D | `HashList<InWorldTowerDefenseSpecial, 4, -1>` type. |
## InWorldTowerDefenseNotifyPacket
Superclass of `Target`. Constructor is inlined in `Target` constructor at `00a85f86`.

| Offset | Size | Name | Confidence | Verification | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| 20 | 4 | op code 3 | H | D | `6` (`0x6`). |
| 24 | 4 |  | L | D | Seemingly always `0`. |
| 28 | 4 |  | L | D | Initialized to `0`. |
| 32 | 4 |  | L | D | Initialized to `vftable`. |
| 36 | 4 |  | L | D | Initialized to `0`. |
| 40 | 4 |  | L | D | Initialized to `0`. |
## InWorldTowerDefenseOptionPacket
| Offset | Size | Name | Confidence | Verification | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| 20 | 4 | op code 3 | H | D | `8` (`0x8`). |
| 24 | 4 |  | L | D | Seemingly always `0`. |
| 28 | 4 |  | L | D | Seemingly always `0`. |
## InWorldTowerDefensePacketTowerTransaction
Constructor is inlined at `00a89546`.

| Offset | Size | Name | Confidence | Verification | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| 20 | 4 | op code 3 | H | D | `5` (`0x5`). |
| 24 | 4 |  | L | D | Seemingly always `0`. |
| 28 | 8 |  | L | D | Likely a GUID. |
| 36 | 8 |  | L | D | Same value as the previous field. |
| 44 | 8 |  | L | D | Same value as the previous field. |
| 52 | 4 |  | L | D | Initialized to 0. |
| 56 | 4 |  | L | D | Initialized to `vftable`. |
| 60 | 4 |  | L | D | Initialized to value at `01c67a0c`. |
| 64 | 4 |  | L | D | Initialized to 0. |
| 68 | 4 |  | L | D | Initialized to 0. |
| 72 | 4 |  | L | D | Initialized to 0. |
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
