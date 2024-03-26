# SPDX-License-Identifier: GPL-2.0
ccflags-y += -I$(src)/ -DWILC_ASIC_A0 -DWILC_DEBUGFS

wilc-objs := cfg80211.o wlan.o wlan_cfg.o \
			hif.o mon.o netdev.o \
			bt.o sysfs.o debugfs.o power.o wilcs02_loopback.o

obj-$(CONFIG_WILC_SDIO) += wilc-sdio.o
wilc-sdio-objs += $(wilc-objs)
wilc-sdio-objs += wilc_sdio.o

obj-$(CONFIG_WILC_SPI) += wilc-spi.o
wilc-spi-objs += $(wilc-objs)
wilc-spi-objs += wilc_spi.o 
