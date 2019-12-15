DEFS = -DCONFIG_OPPO_FINGERPRINT_KERNEL_VER=$(VERSION)
ccflags-y += $(DEFS)

obj-y  += gf_spi.o gf_platform.o gf_netlink.o

ifneq ($(filter MSM_18115 MSM_18501 MSM_18503 MSM_18119 MSM_19061 MSM_19361 MSM_19071 MSM_19081 MSM_19053 MSM_19371 MSM_19688 MSM_19781, $(OPPO_TARGET_DEVICE)),)
ccflags-y += -DUSED_GPIO_PWR
ccflags-y += -DCONFIG_MSM_855
endif

ifneq ($(filter MSM_19081 MSM_19053 MSM_19688 MSM_19781, $(OPPO_TARGET_DEVICE)),)
ccflags-y += -DCONFIG_19081_PWR
endif

ifneq ($(filter MSM_18383, $(OPPO_TARGET_DEVICE)),)
ccflags-y += -DUSED_GPIO_PWR
endif

ifneq ($(filter MSM_19031 MSM_19331 MSM_19111 MSM_19513, $(OPPO_TARGET_DEVICE)),)
ccflags-y += -DAUTO_PWR
ccflags-y += -DCONFIG_MSM_7150
endif

