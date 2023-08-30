# CheckPointProject
This project showcases the development of Linux kernel modules to enhance networking capabilities through NetFilter hooks.
NetFilter is a framework within the Linux kernel that enables various forms of network packet manipulation. 
In this project, we've implemented two separate functionalities using NetFilter hooks: IP logging and a basic firewall.

## IP Logger (netfilter_ip_logger.c)
The netfilter_ip_logger.c module demonstrates IP logging capabilities by intercepting incoming and outgoing network packets and extracting their source
and destination IP addresses. The logged IP addresses are then printed in the kernel logs.
This module provides insights into network traffic patterns and can be a valuable tool for network analysis.

## Firewall (netfilter_firewall.c)
The netfilter_firewall.c module implements a basic firewall using NetFilter hooks. 
It filters incoming and outgoing packets based on a predefined IP address. 
Packets with a specific IP address as the source or destination are dropped, effectively preventing communication with that IP. 
This firewall showcases the potential for implementing packet filtering and security mechanisms using NetFilter.
