obj-m += kernel__.o

all:
	make -C /lib/modules/$(shell uname -r)/build M=$(PWD) modules

user: user.c
	gcc -o user user.c

clean:
	make -C /lib/modules/$(shell uname -r)/build M=$(PWD) clean
	rm user
