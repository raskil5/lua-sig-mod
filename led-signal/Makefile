include $(TOPDIR)/rules.mk

PKG_NAME:=led-signal
PKG_VERSION:=1.0
PKG_RELEASE:=1
PKG_LICENSE:=MIT

include $(INCLUDE_DIR)/package.mk

define Package/led-signal
  SECTION:=utils
  CATEGORY:=Utilities
  TITLE:=LED Signal Indicator
  DEPENDS:=+lua +gcom
endef

define Package/led-signal/install
    $(INSTALL_DIR) $(1)/usr/bin
    $(INSTALL_BIN) $(PKG_BUILD_DIR)/files/usr/bin/led_signal.lua $(1)/usr/bin/led_signal.lua
endef

$(eval $(call BuildPackage,led-signal))
