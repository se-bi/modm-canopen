# Simple SocketCAN on Linux

## Build SocketCAN device

```bash
lbuild build
scons build
```

## Set up virtual SocketCAN

```bash
sudo modprobe vcan
# Create a vcan network interface with a specific name
sudo ip link add dev vcan0 type vcan
sudo ip link set vcan0 up
```

from <https://python-can.readthedocs.io/en/master/interfaces/socketcan.html>
