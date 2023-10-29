# glinet mv1000w ssrplus
# Releases 安装包含:
## 3.216 固件 openwrt-mv1000-emmc-3.216-0321-1679391509.img
## 29个ipk文件 ==> ssrplus
## 安装 opkg install *ipk

# ************** err handling ******************
http://10.0.0.1/cgi-bin/luci/admin/system/opkg
click actions
## update lists...
OPKG Configuration
Below is a listing of the various configuration files used by opkg. Use opkg.conf for global settings and customfeeds.conf for custom repository entries. The configuration in the other files may be changed but is usually not preserved by sysupgrade.

src/gz glinet_kmod https://fw.gl-inet.cn/releases/v19.07.8/kmod-3.0/mvebu/cortexa53

src/gz glinet_packages https://fw.gl-inet.cn/releases/v19.07.8/packages-3.0/mvebu/packages
## install missing pkgs below.
############################## errs ################################
Collected errors:
 * satisfy_dependencies_for: Cannot satisfy the following dependencies for iptables-mod-tproxy:
 * 	kmod-ipt-tproxy
 * opkg_install_cmd: Cannot install package iptables-mod-tproxy.
 * satisfy_dependencies_for: Cannot satisfy the following dependencies for luci-app-ssr-plus:
 * 	coreutils
 * 	coreutils-base64
 * 	libuci-lua
 * 	libudns
 * 	libatomic1
 * 	libmbedtls12
 * 	libcares
 * 	libudns
 * 	libstdcpp6
 * 	boost
 * 	boost-system
 * 	boost-program_options
 * 	boost-date_time
 * opkg_install_cmd: Cannot install package luci-app-ssr-plus
## rerun opkg install *ipk
## reboot
