Minimal Gaia
============


This is a minimal Gaia implementation.

Instructions
------------

### Deploy on hardware using DevTools

Development deployments can be done using DevTools. Enable certified apps for
DevTools using the script provided by
[TWQA/B2G-flash-tool](https://github.com/Mozilla-TWQA/B2G-flash-tool)

```
$ enable_certified_apps_for_devtools.sh
```


### Deploy on hardware as system application using ADB
Push from a Gaia development environment

```
$ APP=system make install-gaia && adb shell stop b2g && adb shell start b2g
```


### Alternative methods

To flash your changes to your device run:

```bash
make install-phone
```

To clear out the whole device and make a fresh build, run:

```bash
make reset-phone
```

