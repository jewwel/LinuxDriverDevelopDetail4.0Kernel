#General Purpose Makefile for Linux Kernel module by guoqingbo

#KERN_DIR = /home/gqb/development/linux-kernel-2.6.37 specific kernel surce code
#KERN_DIR = /usr/src/$(shell uname -r)
KERN_DIR = /lib/modules/$(shell uname -r)/build
obj-m += globalmem6-3-6.o
all:
	make -C $(KERN_DIR) M=$(shell pwd) modules   

clean:                                  
	make -C $(KERN_DIR) M=$(shell pwd) modules clean
	rm -rf modules.order