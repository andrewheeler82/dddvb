#
# Makefile for the ddbridge device driver
#
#NOSTDINC_FLAGS += -I$(KBUILD_EXTMOD)/include -I$(KBUILD_EXTMOD)/include/linux -I$(KBUILD_EXTMOD)/dvb-frontends -I$(KBUILD_EXTMOD)/tuners

ddbridge-objs = ddbridge-main.o ddbridge-hw.o ddbridge-i2c.o ddbridge-ns.o ddbridge-modulator.o ddbridge-core.o ddbridge-ci.o ddbridge-max.o ddbridge-mci.o ddbridge-sx8.o ddbridge-m4.o dvb_netstream.o
octonet-objs = octonet-main.o ddbridge-hw.o ddbridge-i2c.o ddbridge-ns.o ddbridge-modulator.o ddbridge-core.o ddbridge-ci.o ddbridge-max.o ddbridge-mci.o ddbridge-sx8.o ddbridge-m4.o dvb_netstream.o

obj-$(CONFIG_DVB_DDBRIDGE) += ddbridge.o

obj-$(CONFIG_DVB_OCTONET) += octonet.o

#ccflags-y += -Idrivers/media/include/linux/
#ccflags-y += -Idrivers/media/dvb-frontends/
#ccflags-y += -Idrivers/media/tuners/
