#
# Makefile for the linux kernel.
#

# Common support
obj-y := common.o sram.o clock.o devices.o dma.o mux.o gpio.o \
	 usb.o fb.o fb-vram.o fb-vrfb.o io.o
obj-m :=
obj-n :=
obj-  :=

# OCPI interconnect support for 1710, 1610 and 5912
obj-$(CONFIG_ARCH_OMAP16XX) += ocpi.o

obj-$(CONFIG_OMAP_MCBSP) += mcbsp.o

obj-$(CONFIG_CPU_FREQ) += cpu-omap.o
obj-$(CONFIG_OMAP_DM_TIMER) += dmtimer.o
obj-$(CONFIG_OMAP_BOOT_REASON) += bootreason.o
obj-$(CONFIG_OMAP_COMPONENT_VERSION) += component-version.o
obj-$(CONFIG_OMAP_GPIO_SWITCH) += gpio-switch.o
obj-$(CONFIG_OMAP_DEBUG_DEVICES) += debug-devices.o
obj-$(CONFIG_OMAP_DEBUG_LEDS) += debug-leds.o
obj-$(CONFIG_I2C_OMAP) += i2c.o

# OMAP mailbox framework
obj-$(CONFIG_OMAP_MBOX_FWK) += mailbox.o

obj-$(CONFIG_OMAP_PM_NOOP) += omap-pm-noop.o
obj-$(CONFIG_OMAP_PM_SRF) += omap-pm-srf.o \
				resource.o

# OMAP2/3 Display Subsystem
obj-y += dss/

# PSP version information
obj-$(CONFIG_MACH_OMAP3EVM) += psp-version.o
