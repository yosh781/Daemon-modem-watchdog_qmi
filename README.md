 This service is needed in a scenario where the modem hangs up and there is no connection. This can be due to ISP reconnections, due to modem overheating, 
due to modem firmware ....


Modem and network restart daemon for connecting with proto QMI,Openwrt. An alternative to Watchcat.

set up:  qmi-utils

Move script "modem-watchdog_qmi" to   /usr/bin/modem-watchdog_qmi  

chmod +x/usr/bin/modem-watchdog_qmi

Place the file "modem-watchdog_qmi(etcinit.d)" in   /etc/init.d/modem-watchdog_qmi ,   rename to "modem-watchdog_qmi" , 

chmod +x /etc/init.d/modem-watchdog_qmi

/etc/init.d/modem-watchdog_qmi enable

/etc/init.d/modem-watchdog_qmi start
