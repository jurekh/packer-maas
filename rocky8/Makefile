PACKER ?= packer

.PHONY: all clean

all: rocky8.tar.gz

rocky8.tar.gz: clean
	sudo PACKER_LOG=1 ${PACKER} build rocky8.json
	reset

clean:
	sudo ${RM} -rf output-qemu rocky8.tar.gz
