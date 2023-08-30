# mcp-can
CAN library for MCP2515

forked from https://github.com/Longan-Labs/Arduino_CAN_BUS_MCP2515

Added Function ``setClock``

setClock:   allows crystal frequency to be set to various frequencies.

eg   

```
  CANx.setClock(MCP_8MHZ);
  while (CAN_OK != CANx.begin(CAN_500KBPS))
  {
    Serial << "CANx FAIL" << endl;
    delay(100);
  }
  ```

```
enum CAN_CLOCK {
    MCP_20MHZ,
    MCP_16MHZ,
    MCP_8MHZ
};
```
