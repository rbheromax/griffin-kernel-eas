greybus-y :=	core.o		\
		debugfs.o	\
		hd.o		\
		manifest.o	\
		interface.o	\
		bundle.o	\
		connection.o	\
		protocol.o	\
		control.o	\
		svc.o		\
		firmware.o	\
		operation.o

gb-phy-y :=	gpbridge.o	\
		sdio.o	\
		uart.o	\
		pwm.o	\
		gpio.o	\
		i2c.o	\
		spi.o	\
		usb.o

gb-audio-y :=   audio.o \
		audio-gb-cmds.o \
		mods_codec.o

gb-mods-y :=	muc_core.o \
		mods_ap.o \
		muc_gpio.o \
		muc_svc.o \
		mods_init.o \
		muc_spi.o \
		apba.o \
		mods_uart.o \
		mods_uart_pm.o \
		mods_nw.o \
		crc.o

# Prefix all modules with gb-
gb-vibrator-y := vibrator.o
gb-battery-y := battery.o
gb-loopback-y := loopback.o
gb-light-y := light.o
gb-raw-y := raw.o
gb-hid-y := hid.o
gb-es2-y := es2.o
gb-db3-y := db3-platform.o
gb-camera-y := camera.o
gb-vendor-moto-y := vendor_moto.o
gb-ptp-y := ptp.o
gb-camera_ext-y := camera_ext_gb.o camera_ext_mod_v4l2.o camera_ext_ctrls.o
gb-usb_ext-y := usb-ext.o
gb-display-y := display.o
gb-sensors_ext-y := sensors_ext.o sensors_ext_iio.o

obj-$(CONFIG_GREYBUS_MOTOROLA) += greybus.o
#obj-$(CONFIG_GREYBUS_MOTOROLA) += gb-audio.o
obj-$(CONFIG_GREYBUS_MOTOROLA) += gb-battery.o
obj-$(CONFIG_GREYBUS_MOTOROLA) += gb-light.o
obj-$(CONFIG_GREYBUS_MOTOROLA) += gb-hid.o
obj-$(CONFIG_GREYBUS_MOTOROLA) += gb-raw.o
obj-$(CONFIG_GREYBUS_MOTOROLA) += gb-mods.o
obj-$(CONFIG_GREYBUS_MOTOROLA) += gb-vendor-moto.o
obj-$(CONFIG_GREYBUS_MOTOROLA) += gb-ptp.o
obj-$(CONFIG_GREYBUS_MOTOROLA) += gb-camera_ext.o
obj-$(CONFIG_GREYBUS_MOTOROLA) += gb-display.o
obj-$(CONFIG_GREYBUS_MOTOROLA) += gb-usb_ext.o
obj-$(CONFIG_GREYBUS_MOTOROLA) += gb-sensors_ext.o

CONFIG_OPTIONS_ENABLE += LEDS_CLASS_FLASH

#obj-m += gb-phy.o
#obj-m += gb-vibrator.o
#obj-m += gb-loopback.o

# Remove the ES1/2 and db3 host device drivers
#obj-m += gb-es2.o
#obj-m += gb-db3.o
#obj-m += gb-camera.o


# add -Wall to try to catch everything we can.
ccflags-y := -Wall

# needed for trace events
ccflags-y += -I$(src)
