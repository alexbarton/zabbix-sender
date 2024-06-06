#
# Makefile
#

SOURCE_ROOT ?= $(CURDIR)/..

include ../lib/Makefile.ax

install-local:
	install -o $(USER) -g $(GROUP) -m 0644 \
	 zabbix-sender.service zabbix-sender.timer \
	 $(DESTDIR)/etc/systemd/system/
