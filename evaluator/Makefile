TOPTARGETS := all clean

# Filter out power_libs/ from the list of subdirectories
SUBDIRS := $(filter-out power_libs/., $(wildcard */.))
SUBDIRS := $(filter-out scarv_soc/., $(SUBDIRS))

# default:
# 	@echo $(SUBDIRS)

$(TOPTARGETS): $(SUBDIRS)
$(SUBDIRS):
		$(MAKE) -s -C $@ $(MAKECMDGOALS)

.PHONY: $(TOPTARGETS) $(SUBDIRS)