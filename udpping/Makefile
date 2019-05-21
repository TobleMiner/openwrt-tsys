include $(TOPDIR)/rules.mk

PKG_NAME:=udpping
PKG_VERSION:=1
PKG_RELEASE:=1

PKG_SOURCE_PROTO:=git
PKG_SOURCE_URL:=https://github.com/TobleMiner/udpping.git
PKG_SOURCE_VERSION:=HEAD

#PKG_BUILD_DIR:=$(BUILD_DIR)/$(PKG_NAME)

include $(INCLUDE_DIR)/package.mk

define Package/udpping
	SECTION:=net
	CATEGORY:=Network
	TITLE:=Simple UDP-based network testing utility
endef

define Package/udpping/install
	$(INSTALL_DIR) $(1)/usr/bin
	$(INSTALL_BIN) $(PKG_INSTALL_DIR)/usr/bin/udpping $(1)/usr/bin/install
endef

$(eval $(call BuildPackage,udpping))
