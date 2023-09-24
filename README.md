## Cloudrack Umbrel Community App Store

You can use the Umbrel CLI as described below.

To add an app store:
```shell
sudo ~/umbrel/scripts/repo add https://github.com/cloudrack-ca/cloudrack-umbrel-apps.git
```
```shell
sudo ~/umbrel/scripts/repo update
```

To install an app from the app store

WordPress
```shell
sudo ~/umbrel/scripts/app install cloudrack-wordpress
```
KasmWeb
```
sudo ~/umbrel/scripts/app install cloudrack-kasm
```
To remove an app store:
```shell
sudo ~/umbrel/scripts/repo remove https://github.com/cloudrack-ca/cloudrack-umbrel-apps.git
```
