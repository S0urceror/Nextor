# Top level makefile for Nextor.
# It will build the kernel ROM files, NEXTOR.SYS and the command line tools.
# The generated files will be copied to bin/kernels and bin/tools.
# The makefiles on each directory can be used independently as well.

export PATH := /Users/mario/Development/msx/Compilers/sjasm:/Users/mario/Development/msx/Compilers/sdcc-4.1.0/bin:/Users/mario/Development/msx/Compilers/M80.net:/opt/homebrew/opt/binutils/bin:/Users/mario/Development/MSX/OS/Nextor/buildtools/macos:$(PATH)

all:
	$(MAKE) -C kernel
	$(MAKE) -C command/msxdos
	$(MAKE) -C tools
	$(MAKE) -C tools/C

.PHONY: clean

clean:
	$(MAKE) -C kernel clean
	$(MAKE) -C command/msxdos clean
	$(MAKE) -C tools clean
	$(MAKE) -C tools/C clean
