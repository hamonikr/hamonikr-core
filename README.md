# hamonikr-server-settings

Adjustments to the Ubuntu package base for HamoniKR Linux
These adjustments modify some unwanted behaviors of the Ubuntu package base and are specific to this base.

하모니카 서버에 필요한 환경으로 조정하는 시스템 서비스 패키지

# Installation

```
wget -qO- https://pkg.hamonikr.org/add-hamonikr-server-entjin.apt | sudo -E bash -

sudo apt install hamonikr-system-settings
```

# Adjustment Works
etc/apt/apt.conf.d/00hamonikr
etc/apt/preferences.d/hamonikr.pref
etc/default/grub.d/50_hamonikr.cfg
etc/hamonikr/distribution.ini
etc/hamonikr/vendor-firefox.js
etc/ImageMagick-6/policy.xml
etc/lightdm/lightdm.conf.d/90-hamonikr.conf
etc/skel/.config/albert/*
etc/skel/.hamonikr/default_dconf
etc/skel/.hamonikr/hamonikr-jin-terminal.dconf
etc/timeshift/restore-hooks.d/60_hamonikr
etc/xdg/autostart/*
usr/bin/hamonikr-system-settings
usr/bin/hamonikr-system-start
usr/bin/hamonikr-system-stop
usr/bin/update-default-browser
usr/bin/update-firefox-setting
usr/bin/update-grub-title.py
usr/bin/update-lightdm-display-setting
usr/local/bin/auto-display-setup
usr/local/bin/update-dconf-setting
usr/share/fonts/truetype/droidmono/DroidSansMono.ttf
usr/share/cinnamon/applets/*
usr/share/locale/ko/LC_MESSAGES/*
usr/share/mime/packages/alzip.xml
usr/share/mint-mirrors/linuxmint.list
usr/share/nemo/actions/*
usr/share/plymouth/themes/*

# Issues

https://hamonikr.org/
