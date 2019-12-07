include $(TOPDIR)/rules.mk

PKG_NAME:=gpio_poe
PKG_VERSION:=1
PKG_RELEASE:=1

include $(INCLUDE_DIR)/package.mk

define Package/gpio_poe
	SECTION:=utils
	CATEGORY:=Utilities
	TITLE:=GPIO PoE - Controlling PoE ports via GPIOs
endef

define Build/Compile
endef

define Package/gpio_poe/install
	$(INSTALL_DIR) $(1)/etc/init.d
	$(INSTALL_BIN) ./files/etc/init.d/gpio_poe $(1)/etc/init.d/gpio_poe
endef

$(eval $(call BuildPackage,gpio_poe))
