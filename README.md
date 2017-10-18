# njitis620

#  Prior to First Github Upload, - Spun up Linx VM, Set Static IP, Installed Nagios with basic Config 
#  Enabled SNMP on Main Router, and Enabled Basic SNMP on topsite Host
#  Nagios using nsclient++ for windows hosts, SNMP for router and media …
#  https://imgur.com/a/QjAbQ
#  Finally got Plugin to work, plugin checkuptime via SNMP , removed non…
#  e working network monitoring on port https://imgur.com/a/UVAnZ
#  Added SNMP Monitoring health for router using swap space & IN and OUT…
#  octets https://imgur.com/a/op7Iw
#  Added OMEGA via NSClient++, Monitors, Disk/cpu/memory, Will also moni…
#  tor backup service and disk IO - https://imgur.com/1auTuw7
#  I then created a custom Command in the Nagios Commands to allow this new plugin to be used,
#  I then defined the host and the service to monitor the disk IO of the test media server and alert to warn @ 10 % usage,
#  and Critial @ 100% usage - https://imgur.com/b0ubgt5
#
#
#  Project Deliverables
#  
#  Identity one of your services that logs errors.  Configure Nagios to alert properly on that data - 
#  -  This was done using NS++ agent on the website site, to monitor the Running status of "Plex update Service", also to watch out of errors that the service will log in the windows event log, I have created a SNMP trap that will flag if any of the event codes besides "normal"
#  Identity a service that uses SNMP to broadcast its health, configure Nagios to monitor the health of that service properly
#  - This is done by enabling SNMP on my Main Router - rt-n66u, I was then able to monitor Uptime and incoming and going octets on my WAN adaptor.
#  Configure Nagios to monitor the InOcts/OutOcts of one of the media servers.  Set warning thresholds to alert on them
#  - This is was done by adding the "systat" module using apt-get on my Test linux Media Server, Then By getting the nagios plugin, "check_diskstat"
#  I then created a custom Command in the Nagios Commands to allow this new plugin to be used, I then defined the host and the service to monitor the disk IO of the test media server and aleart to warn @ 10 % usage, and Critial @ 100% usage - https://imgur.com/b0ubgt5







