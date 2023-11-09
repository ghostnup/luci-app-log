# luci-app-log
Advanced syslog and kernel log (tail, search, etc) for LuCI (OpenWrt webUI).

OpenWrt >= 19.07.

Supported LuCI themes: luci-theme-bootstrap, luci-theme-material, luci-theme-openwrt-2020.

## Installation notes

**OpenWrt >= 21.02:**

    wget --no-check-certificate -O /tmp/luci-app-log_0.8-0_all.ipk https://github.com/gSpotx2f/packages-openwrt/raw/master/current/luci-app-log_0.8-0_all.ipk
    opkg install /tmp/luci-app-log_0.8-0_all.ipk
    rm /tmp/luci-app-log_0.8-0_all.ipk
    /etc/init.d/rpcd restart

i18n-ru:

    wget --no-check-certificate -O /tmp/luci-i18n-log-ru_0.8-0_all.ipk https://github.com/gSpotx2f/packages-openwrt/raw/master/current/luci-i18n-log-ru_0.8-0_all.ipk
    opkg install /tmp/luci-i18n-log-ru_0.8-0_all.ipk
    rm /tmp/luci-i18n-log-ru_0.8-0_all.ipk

**OpenWrt 19.07:**

    wget --no-check-certificate -O /tmp/luci-app-log_0.4-6_all.ipk https://github.com/gSpotx2f/packages-openwrt/raw/master/19.07/luci-app-log_0.4-6_all.ipk
    opkg install /tmp/luci-app-log_0.4-6_all.ipk
    rm /tmp/luci-app-log_0.4-6_all.ipk
    /etc/init.d/rpcd restart

i18n-ru:

    wget --no-check-certificate -O /tmp/luci-i18n-log-ru_0.4-6_all.ipk https://github.com/gSpotx2f/packages-openwrt/raw/master/19.07/luci-i18n-log-ru_0.4-6_all.ipk
    opkg install /tmp/luci-i18n-log-ru_0.4-6_all.ipk
    rm /tmp/luci-i18n-log-ru_0.4-6_all.ipk

## Screenshots:

Kernel log:

![](https://github.com/gSpotx2f/luci-app-log/blob/master/screenshots/01.jpg)

System log (logd):

![](https://github.com/gSpotx2f/luci-app-log/blob/master/screenshots/02.jpg)

System log (syslog-ng):

![](https://github.com/gSpotx2f/luci-app-log/blob/master/screenshots/03.jpg)

## Mod lines (OpenWrt >= 21.02):

    wget --no-check-certificate -O /www/luci-static/resources/view/log/log-widget.js https://github.com/gSpotx2f/luci-app-log/raw/master/dev-mods-examples/mod-lines/htdocs/luci-static/resources/view/log/log-widget.js

![](https://github.com/gSpotx2f/luci-app-log/blob/master/dev-mods-examples/mod-lines/screenshots/01.jpg)

## Mod textarea (OpenWrt >= 21.02):

    wget --no-check-certificate -O /www/luci-static/resources/view/log/log-widget.js https://github.com/gSpotx2f/luci-app-log/raw/master/dev-mods-examples/mod-textarea/htdocs/luci-static/resources/view/log/log-widget.js
    wget --no-check-certificate -O /www/luci-static/resources/view/log/log-widget.js https://github.com/gSpotx2f/luci-app-log/raw/master/dev-mods-examples/mod-textarea/htdocs/luci-static/resources/view/log/dmesg.js
    wget --no-check-certificate -O /www/luci-static/resources/view/log/log-widget.js https://github.com/gSpotx2f/luci-app-log/raw/master/dev-mods-examples/mod-textarea/htdocs/luci-static/resources/view/log/syslog.js

![](https://github.com/gSpotx2f/luci-app-log/blob/master/dev-mods-examples/mod-textarea/screenshots/01.jpg)
