# Scaled Up Web Infrastructure

![Image of a scaled up web infrastructure](3-scale_up.jpg)

[Visit Board](https://wbd.ms/share/v2/aHR0cHM6Ly93aGl0ZWJvYXJkLm1pY3Jvc29mdC5jb20vYXBpL3YxLjAvd2hpdGVib2FyZHMvcmVkZWVtLzM1NmEyMDBlZjNhNTQ0ODc4ZjcyYTI4ZTU0NGRiYzJiX0JCQTcxNzYyLTEyRTAtNDJFMS1CMzI0LTVCMTMxRjQyNEUzRF85NDA4MGRhNS03MWEwLTQxMjYtODRmNi1jNDA2NWEzMTljYWI=)

## Description

This web infrastructure is a scaled up version of the infrastructure described [here](2-secured_and_monitored_web_infrastructure.md). In this version, all SPOFs have been removed and each of the major components (web server, application server, and database servers) have been moved to separate GNU/Linux servers. The SSL protection isn't terminated at the load-balancer and each server's network is protected with a firewall and they're also monitored.

## Specifics About This Infrastructure

+ The addition of a firewall between each server.<br/>This protects each server from unwanted and unauthorized users rather than protecting a single server.

## Issues With This Infrastructure

+ High maintenance costs.<br/>Moving each of the major components to its own server, means that more servers would have to be bought and the company's electricity bill would rise along with the introduction of new servers. Some of the company's funds would have to be used to buy the servers and pay for the electricity consumption needed to keep the servers (including the new and old ones) running.
