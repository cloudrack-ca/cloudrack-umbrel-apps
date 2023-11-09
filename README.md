# Cloudrack Umbrel Community App Store

- need support? request a new app? request an app update?
  Join my [Discord](https://discord.gg/tEz2R6JQu8)

You can use the Umbrel CLI as described below.

# IMPORTANT NOTICE 
# PLESK IS NOT RUNNABLE CURRENTLY AND WILL NOT UNINSTALL VIA UI - IF YOU ARE HAVING THESE ISSUES PLEASE MESSAGE ME ON DISCORD

---
# To add an app store:
```shell
sudo ~/umbrel/scripts/repo add https://github.com/cloudrack-ca/cloudrack-umbrel-apps.git
```
```shell
sudo ~/umbrel/scripts/repo update
```
---
# To install an app from the app store

### To Install -> [`WordPress`](https://github.com/cloudrack-ca/cloudrack-umbrel-apps/tree/master/cloudrack-wordpress)
```shell
sudo ~/umbrel/scripts/app install cloudrack-wordpress
```
### To Install -> [`KasmWeb`](https://github.com/cloudrack-ca/cloudrack-umbrel-apps/tree/master/cloudrack-kasm)
```
sudo ~/umbrel/scripts/app install cloudrack-kasm
```
### To Install -> [`Plesk`](https://github.com/cloudrack-ca/cloudrack-umbrel-apps/tree/master/cloudrack-plesk)
```
sudo ~/umbrel/scripts/app install cloudrack-plesk
```
---
# To remove an app store:
```shell
sudo ~/umbrel/scripts/repo remove https://github.com/cloudrack-ca/cloudrack-umbrel-apps.git
```
