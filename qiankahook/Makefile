THEOS_DEVICE_IP = 192.168.0.103
ARCHS = armv7 arm64
TARGET = iphone:latest:8.0

include theos/makefiles/common.mk

TWEAK_NAME = qiankahook
qiankahook_FILES = Tweak.xm
qiankahook_FRAMEWORKS = UIKit Security

include $(THEOS_MAKE_PATH)/tweak.mk

after-install::
	install.exec "killall -9 QiankaKey"
