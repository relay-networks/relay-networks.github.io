# Scans through the relay network

The two files (webserver-log, scan-results) can be combined by using the timestamp of the scan-results file and join it with the timestamp encoded in the request url which is last column of the webserver-log file.
The send column of the webserver-log file contains the egress IP address as seen by our server.
The scan-results file's egress IP address is the one obtained by querying ipecho.net

The scan on the 09.05 did use the fixed DNS setup while the scan on the 06.09 used the open setup.
