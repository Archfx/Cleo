#Update the module name for the DuT
MODULE=xc_aessub


VMODULE=V$(MODULE)
DUTPATH=../../eut/xcrypto/rtl/$(MODULE)/$(MODULE).v
DUTPATH+=../../eut/xcrypto/rtl/xc_aessub/xc_aessub_sbox.v
POWER_LIBS=../power_libs


SOC=scarv_soc
SOC_DIR=../$(SOC)

APP_NAME=aes
FIRMWARE=$(SOC_DIR)/firmware
APP_SRC=$(FIRMWARE)/aes.S


include $(POWER_LIBS)/tvla-fu.mk
