PROJECT_NAME = $(subst MSM_,,$(OPPO_TARGET_DEVICE))

DEFS = -DCONFIG_OPPO_FINGERPRINT_PROJCT=$(PROJECT_NAME)
ccflags-y += $(DEFS)

DEFS = -DCONFIG_OPPO_FINGERPRINT_KERNEL_VER=$(VERSION)
ccflags-y += $(DEFS)

obj-y  += gf_spi.o gf_platform.o gf_netlink.o
