# KasmWeb On Umbrel
---
# Install Kasmweb on your Umbrel with 
```shell
sudo ~/umbrel/scripts/app install cloudrack-kasm
```
# Volumes Used
---
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
