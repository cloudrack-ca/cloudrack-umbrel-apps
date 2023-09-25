# KasmWeb On Umbrel
---
# Install Kasmweb on your Umbrel with 
```shell
sudo ~/umbrel/scripts/app install cloudrack-kasm
```
---
# Uninstall Kasmweb on your Umbrel with 
```shell
sudo ~/umbrel/scripts/app uninstall cloudrack-kasm
```
---
# Reinstall Kasmweb on your Umbrel with 
- Calls 'uninstall', followed by 'install' for an app
```shell
sudo ~/umbrel/scripts/app reinstall cloudrack-kasm
```
---
# Volumes Used
```yaml
    volumes:
      - type: volume
        source: kasm_opt
        target: /opt
      - type: volume
        source: kasm_profiles
        target: /profiles
      - type: volume
        source: kasm_dev_input
        target: /dev/input
      - type: volume
        source: kasm_run_udev_data
        target: /run/udev/data
      - type: bind
        source: /sys/kernel/security
        target: /sys/kernel/security
        read_only: true
```
```yaml
volumes:
  kasm_opt:
  kasm_profiles:
  kasm_dev_input:
  kasm_run_udev_data:
```
---
# Ports Used
```yaml
    ports:
      - target: 3000
        published: "3000"
        protocol: tcp
      - target: 4443
        published: "4443"
        protocol: tcp
```
---
# Temp File System - 1GB On Alpine
```yaml
  tmpfs:
    image: alpine
    command: sh -c "sleep 9999999999d"
    volumes:
      - type: tmpfs
        target: /tmpfs
        tmpfs:
          size: 1g
```
