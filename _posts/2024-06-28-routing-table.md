---
layout: post
title:  "Routing Table"
date:   2024-06-28 12:11:42 -0700
categories: jekyll update
---

All network devices, whether they are hosts, routers, or other types of network nodes such as network attached printers, need to make decisions about where to route TCP/IP data packets. The routing table provides the configuration information required to make those decisions.A routing table similar to the very simple one in Figure 1 is used to define the single route available to a typical local host and to determine whether to send packets to the default gateway router. The route -n command lists the routing table; the -n option displays the results as IP addresses only and does not attempt to perform a DNS lookup which would replace the IP address with hostnames if they are available. The netstat -rn command produces very similar results.

[root@host1 ~]# route -n
Kernel IP routing table
Destination     Gateway         Genmask         Flags Metric Ref    Use Iface
0.0.0.0         192.168.0.254   0.0.0.0         UG    100    0        0 eno1
192.168.0.0     0.0.0.0         255.255.255.0   U     100    0        0 eno1

2024-05-31-your-new-blog-post.md
