
| Offset | Size | Name | Confidence | Verification | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| 0 | 4 | op code | H | D | `39` (`0x27`).  |
| 4 | 4 | op code 2 | H | D | Distinguishes subclasses/children of `BaseMiniGamePacket` from other children. |
| 8 | 4 | match ID | L | D | `-1`  (`0xffffffff`) when unused. The name is based on the value being present for Saber Strike packets that would be associated with a match (`GameOverPacket`, `KillPacket`, `ObfuscatedScorePacket`, `ThrowKillPacket`) and not Saber Strike boost packets that are not specific to a match. However, the value `0` is used for most Attack Cruiser (`StarDestroyer`) packets. |
| 12 | 4 |  |  | D | `-1` (`0xffffffff`) when unused. Definitely used by TCG. Unused by Galactic Forces, Speeder Racing, and Saber Strike. |
| 16 | 4 | op code 3 | H | D | `-1` (`0xffffffff`) when unused. Distinguishes grandchildren of `BaseMiniGamePacket` from other grandchildren (ex: subclasses of `BaseStarDestroyerPacket`). |
## MiniGameBoostActivatedPacket

## MiniGameCreateGameResultPacket

## MiniGameDataLockedPacket

## MiniGameDataPacket

## MiniGameDataUnlockedPacket

## MiniGameGameEndScorePacket

## MiniGameGameOverPacket

## MiniGameGroupInfoPacket

## MiniGameInfoPacket

## MiniGameKnockOutPacket

## MiniGameLootWheelOnRotationStoppedPacket

## MiniGameMessagePacket

## MiniGamePayloadPacket

## MiniGameRewardStatusPacket

## MiniGameStarsEarnedPacket

## RequestTCGChallengePacket

## TradingCardStartGamePacket
