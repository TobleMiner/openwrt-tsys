include $(TOPDIR)/rules.mk

PKG_NAME:=udpping
PKG_VERSION:=2
PKG_RELEASE:=1

PKG_SOURCE_PROTO:=git
PKG_SOURCE_URL:=https://github.com/TobleMiner/udpping.git
PKG_SOURCE_VERSION:=e38f75a6199296ff25f51112215159cfb6dc7d13

include $(INCLUDE_DIR)/package.mk

define Package/udpping
	SECTION:=net
	CATEGORY:=Network
	TITLE:=Simple UDP-based network testing utility
endef

define Package/udpping/install
	$(INSTALL_DIR) $(1)/usr/bin
	$(INSTALL_BIN) $(PKG_BUILD_DIR)/udpping $(1)/usr/bin/udpping
endef

$(eval $(call BuildPackage,udpping))
