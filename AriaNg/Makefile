#

include $(TOPDIR)/rules.mk

PKG_NAME:=aria-ng
PKG_VERSION:=0.4.0
PKG_RELEASE:=1

PKG_SOURCE:=aria-ng-$(PKG_VERSION).zip
PKG_SOURCE_URL:=https://github.com/mayswind/AriaNg/releases/download/$(PKG_VERSION)/
PKG_MD5SUM:=74e76d435dcd8c62b027938133b6417af989a28d278c86fde3b5a7a9c2ecb8fb
PKG_CAT:=unzip

PKG_LICENSE:=MIT
PKG_MAINTAINER:=akaxxi


include $(INCLUDE_DIR)/package.mk

define Package/aria-ng
	SECTION:=net
	CATEGORY:=Network
	TITLE:=A web frontend making aria2 easier to use
	URL:=https://github.com/mayswind/AriaNg
	PKGARCH:=all
endef

define Package/aria-ng/description
AriaNg is a web frontend making aria2 easier to use. 
AriaNg is written in pure html & javascript. 
AriaNg uses responsive layout, and supports any desktop or mobile devices.
endef

define Build/Compile
endef

define Package/aria-ng/install
	$(INSTALL_DIR) $(1)/www/ariang
	$(CP) $(BUILD_DIR)/{css,fonts,js,langs} $(1)/www/ariang
	$(CP) $(BUILD_DIR)/{index.html,index.manifest,LICENSE,robots.txt} $(1)/www/ariang
endef

$(eval $(call BuildPackage,aria-ng))
