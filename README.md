 This service is needed in a scenario where the modem hangs up and there is no connection. This can be due to ISP reconnections, due to modem overheating, 
due to modem firmware ....


Modem and network restart daemon for connecting with proto QMI,Openwrt. An alternative to Watchcat.

install the packages:  qmi-utils  comgt

Move script "modem-watchdog_qmi" to   /usr/bin/modem-watchdog_qmi  

Place the file "modem-watchdog" in   /etc/init.d/modem-watchdog 

chmod +x /etc/init.d/modem-watchdog

chmod +x /usr/bin/modem-watchdog_qmi

/etc/init.d/modem-watchdog enable

/etc/init.d/modem-watchdog start
