-include $(SUBDIRS)/../build_mode

SCST_INC_DIR := $(SUBDIRS)/../../scst/include/

SRPTFLAGS = -DCONFIG_SCST_TRACING -DCONFIG_SCST_DEBUG \
	-DCONFIG_SCST_EXTRACHECKS -fno-inline -fno-inline-functions
SRPTFLAGSRELEASE = -DCONFIG_SCST_TRACING
SRPTFLAGSPERF =
EXTRA_CFLAGS +=  -I$(SCST_INC_DIR) $(SRPTFLAGS$(BUILDMODE))

#EXTRA_CFLAGS += -Wextra -Wno-unused-parameter

obj-m		+= ib_srpt.o
