# dummy_hcd

DKMS for Dummy/Loopback USB host and device emulator driver.

# Install

## Clone

```bash
git clone https://github.com/0prichnik/dummy_hcd.git
```

## Update source up to running kernel version

```bash
make update
```

## Add to DKMS

```bash
make dkms
```

# Load

Emulate one USB2 connected device:

```bash
sudo modprobe dummy_hcd is_high_speed=1
```

# Remove

```bash
sudo dkms remove dummy_hcd/0.1 --all
```
