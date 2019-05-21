include $(TOPDIR)/rules.mk

PKG_NAME:=udpping
PKG_VERSION:=1
PKG_RELEASE:=1

PKG_SOURCE_PROTO:=git
PKG_SOURCE_URL:=https://github.com/TobleMiner/udpping.git
PKG_SOURCE_VERSION:=HEAD

PKG_INSTALL:=1

include $(INCLUDE_DIR)/package.mk

define Package/udpping
	SECTION:=net
	CATEGORY:=Network
	TITLE:=Simple UDP-based network testing utility
endef

$(eval $(call BuildPackage,udpping))
