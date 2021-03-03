# hamonikr-core

하모니카 서버에 필요한 환경으로 조정하는 시스템 서비스 패키지

# Installation

```
wget -qO- https://pkg.hamonikr.org/add-hamonikr-server-entjin.apt | sudo -E bash -

sudo apt install hamonikr-system-settings
```

## Adjustment Works
```
### APT 관련 설정
etc/apt/apt.conf.d/00hamonikr
etc/apt/preferences.d/hamonikr.pref

### grub Title 
etc/default/grub.d/50_hamonikr.cfg

### 파이어폭스 관련 설정
etc/hamonikr/distribution.ini
etc/hamonikr/vendor-firefox.js

### 이미지 변환 설정
etc/ImageMagick-6/policy.xml

### lightdm  
etc/lightdm/lightdm.conf.d/90-hamonikr.conf

### 기본 프로파일
etc/skel/.config/albert/*
etc/skel/.hamonikr/default_dconf
etc/skel/.hamonikr/hamonikr-jin-terminal.dconf

### 백업설정
etc/timeshift/restore-hooks.d/60_hamonikr

### 자동 시작 프로그램
etc/xdg/autostart/*

### 데몬 서비스
usr/bin/hamonikr-system-settings
usr/bin/hamonikr-system-start
usr/bin/hamonikr-system-stop

### 필요한 설정 실행 명령셋
usr/bin/update-default-browser
usr/bin/update-firefox-setting
usr/bin/update-grub-title.py
usr/bin/update-lightdm-display-setting
usr/local/bin/auto-display-setup
usr/local/bin/update-dconf-setting

### 변경필요한 리소스
usr/share/fonts/truetype/droidmono/DroidSansMono.ttf
usr/share/cinnamon/applets/*
usr/share/locale/ko/LC_MESSAGES/*
usr/share/mime/packages/alzip.xml
usr/share/mint-mirrors/linuxmint.list
usr/share/nemo/actions/*
usr/share/plymouth/themes/*
```

# Issues

https://hamonikr.org/
