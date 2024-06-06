# Zabbix Sender: Periodically push Zabbix items from spool files to the server

The _Zabbix Sender_ is meant to be periodically run, for example every few
minutes, and pushes all Zabbix _items_ which have been accumulated in one ore
more _spool files_ to the Zabbix server using the `zabbix_send`(1) command.

This was it is very easy to cope with multiple values, even from different
sources, and not lose items when the system is offline or other errors occur:
the _Zabbix Sender_ retries sending out items until it succeeds.
