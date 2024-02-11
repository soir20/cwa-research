Packet information is presented with tables of the following structure:

| Offset | Size | Name | Confidence | Verification | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| offset within the packet buffer in bytes | field size in bytes | field name | H - high confidence in the name, close to certain<br>L - low confidence in the name, a guess  | D - verified with decompiler<br>L - verified with packet logs or debugger  | Typical values. rationale for the name, or other relevant details |

When fields prior to the first offset given are not specified, they are inherited from the parent class. Addresses are based on the 2014 Clone Wars Adventures client (SHA-256: `c02f3c8a1be8dc28e517a29158c956c16393eb1def4870b0813775c69a62d2dd`).