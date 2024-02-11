| Offset | Size | Name | Confidence | Verification | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| 4 | 4 | op code 2 | H | D | `63` (`0x3f`). |
| 8 | 4 | match ID | L | D | Unused. Always `-1` (`0xffffffff`). |
| 12 | 4 |  |  | D | Unused. Always `-1` (`0xffffffff`). |
| 16 | 4 | op code 3 | H | D | `-1` (`0xffffffff`) when unused. Distinguishes children of `BaseMiniGameBossPacket` from other children. |
## MiniGameBossDeletePacket
| Offset | Size | Name | Confidence | Verification | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| 16 | 4 | op code 3 | H | D | `2` (`0x2`). |
| 20 | 4 |  | L | D | Initialized to `0`. Set at `007c361d` based on the parameters to the `BaseClient`'s packet reception method. |
## MiniGameBossUpdatePacket
| Offset | Size | Name | Confidence | Verification | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| 16 | 4 | op code 3 | H | D | `1` (`0x1`). |
| 20 | 4 |  | L | D | Initialized to `0`. |
| 24 | 4 |  | L | D | Initialized to `0`. |
| 28 | 4 |  | L | D | Initialized to `0`. 
