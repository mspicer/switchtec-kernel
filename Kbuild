LINUXINCLUDE := -I$(src) $(LINUXINCLUDE)

obj-m := switchtec.o

# Only build NTB driver if NTB support is available in the kernel
ifneq ($(CONFIG_NTB),)
obj-m += ntb_hw_switchtec.o
endif

ccflags-y := -Wall -Werror -Werror=implicit-function-declaration
