## Cloudrack Umbrel Community App Store

You can use the Umbrel CLI as described below.

To add an app store:
```
sudo ~/umbrel/scripts/repo add https://github.com/cloudrack-ca/cloudrack-umbrel-apps.git

sudo ~/umbrel/scripts/repo update
```

To install an app from the app store
```
sudo ~/umbrel/scripts/app install cloudrack-wordpress
```

To remove an app store:
```
sudo ~/umbrel/scripts/repo remove https://github.com/cloudrack-ca/cloudrack-umbrel-apps.git
```
