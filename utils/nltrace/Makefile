#
# Copyright (C) 2013-2015 OpenWrt.org
# Copyright (C) 2017 Daniel Engberg <daniel.engberg.lists@pyret.net>
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk
PKG_MAINTAINER:=Christof Schulze <christof.schulze@gmx.net>
PKG_NAME:=nltrace
PKG_SOURCE_DATE:=2018-03-19
PKG_SOURCE_PROTO:=git
PKG_SOURCE_URL:=https://github.com/socketpair/nltrace.git
PKG_SOURCE_VERSION:=1f6eae759c85a7e04c47dc203d282bad96f927d5

include $(INCLUDE_DIR)/package.mk

define Package/nltrace
  SECTION:=utils
  CATEGORY:=Utilities
  TITLE:=nltrace - a netlink tracing tool
  DEPENDS:= +libnl
endef

define Package/nltrace/description
	nltrace is a netlink tracing tool
endef

define Package/nltrace/install
	$(INSTALL_DIR) $(1)/usr/sbin
	$(INSTALL_BIN) $(PKG_BUILD_DIR)/nltrace $(1)/usr/sbin/
endef

$(eval $(call BuildPackage,nltrace))
