#
# Copyright (C) 2006-2008 OpenWrt.org
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#
include $(TOPDIR)/rules.mk

ARCH:=mipsel
BOARD:=bcm47xx
BOARDNAME:=Broadcom BCM47xx/53xx (MIPS)
FEATURES:=squashfs usb
SUBTARGETS:=generic mips74k legacy

KERNEL_PATCHVER:=5.4
KERNEL_TESTING_PATCHVER:=5.4

define Target/Description
	Build firmware images for Broadcom based BCM47xx/53xx routers with MIPS CPU, *not* ARM.
endef

include $(INCLUDE_DIR)/target.mk

DEFAULT_PACKAGES += swconfig nvram otrx \
	kmod-leds-gpio kmod-gpio-button-hotplug

$(eval $(call BuildTarget))
