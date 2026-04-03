include $(TOPDIR)/rules.mk

ARCH:=aarch64
BOARD:=qualcommax
BOARDNAME:=Qualcomm Atheros 802.11ax WiSoC-s
FEATURES:=squashfs ramdisk fpu nand rtc emmc
KERNELNAME:=Image
CPU_TYPE:=cortex-a53
SUBTARGETS:=ipq807x ipq60xx ipq50xx

KERNEL_PATCHVER:=6.12

include $(INCLUDE_DIR)/target.mk
DEFAULT_PACKAGES += \
	autocore cpufreq luci uboot-envtools \
	kmod-phy-qca83xx \
	kmod-gpio-button-hotplug kmod-leds-gpio \
	kmod-qca-nss-dp kmod-qca-nss-ecm \
	kmod-qca-ssdk kmod-qca-nss-drv \
	kmod-qca-nss-drv-pppoe kmod-qca-nss-drv-bridge-mgr

$(eval $(call BuildTarget))
