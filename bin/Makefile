#
# Makefile
#

SOURCE_ROOT ?= $(CURDIR)/..

include ../lib/Makefile.ax

install-local:
	install -o $(USER) -g $(GROUP) -m 0755 \
	 zabbix-sender $(DESTDIR)$(PREFIX)/sbin/zabbix-sender
