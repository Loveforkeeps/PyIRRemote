# PyIRRemote
MicroPython module for receiving and sending IR remote control signals (NEC format) on a ESP32



### Using

receiver:

```python
from IRReceiver import IRReceiver

receiver = IRReceiver(33)
receiver.callback = print
receiver.daemon()
```



sender:

```python
from IRReceiver import IRSender

sender = IRSender(27)
sender.sender('c3f9070005000200000400a0e2')
```

