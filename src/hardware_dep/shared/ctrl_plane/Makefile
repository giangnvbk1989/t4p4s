CC=gcc
CFLAGS=-Wall -pthread -std=c99
LIB=

all: dpdk_portfwd_controller dpdk_l2fwd_controller dpdk_l3fwd_controller

dpdk_portfwd_controller:
	$(CC) $(CFLAGS) $(LIB) handlers.c controller.c messages.c sock_helpers.c threadpool.c fifo.c dpdk_portfwd_controller.c -o dpdk_portfwd_controller

dpdk_l2fwd_controller:
	$(CC) $(CFLAGS) $(LIB) handlers.c controller.c messages.c sock_helpers.c threadpool.c fifo.c dpdk_l2fwd_controller.c -o dpdk_l2fwd_controller

dpdk_l3fwd_controller:
	$(CC) $(CFLAGS) $(LIB) handlers.c controller.c messages.c sock_helpers.c threadpool.c fifo.c dpdk_l3fwd_controller.c -o dpdk_l3fwd_controller

clean:
	rm -f dpdk_portfwd_controller dpdk_l2fwd_controller dpdk_l3fwd_controller

