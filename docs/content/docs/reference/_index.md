# Packet Reference

## Communication Parameters

The Door Lock and Module communicates over UART using the following parameters:

- **Baud Rate**: 9600
- **Data Bits**: 8
- **Parity**: None
- **Stop Bits**: 1
- **Flow Control**: None

## Frame Format

Each UART transmission follows a specified frame format:

```
SYNC | START | LEN | CMD | DATA | CHECKSUM
```

Both Door Lock and Module uses the same frame format but with **different sync bit**.

| Field    | Description                                     |
| -------- | ----------------------------------------------- |
| SYNC     | Door Lock - `0xFF 0xFF 0xFF`<br>Module - `0xFF` |
| START    | Constant - `0x48`                               |
| LEN      | Length of `CMD` + `PAYLOAD`                     |
| CMD      | Command ID                                      |
| PAYLOAD  | Command-specific data                           |
| CHECKSUM | `(LEN + CMD + PAYLOAD) & 0xFF`                  |
