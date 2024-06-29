---
layout: post
title:  "Configuring IP Network with nmcli (based on VPN issues)"
date:   2024-06-28 12:11:42 -0700
categories: Networking
---

### Configuring IP Networking with nmcli

The nmcli (NetworkManager Command Line Interface) command-line utility is used for controlling NetworkManager and reporting network status. It can be utilized as a replacement for nm-applet or other graphical clients. See Section 2.5, “NetworkManager Tools”. nmcli is used to create, display, edit, delete, activate, and deactivate network connections, as well as control and display network device status.

The nmcli utility can be used by both users and scripts for controlling NetworkManager:

For servers, headless machines, and terminals, nmcli can be used to control NetworkManager directly, without GUI, including creating, editing, starting and stopping network connections and viewing network status.
For scripts, nmcli supports a terse output format which is better suited for script processing. It is a way to integrate network configuration instead of managing network connections manually.
The basic format of a nmcli command is as follows:

<pre class=terminal>
nmcli -p device
=====================
  Status of devices
=====================
DEVICE  TYPE      STATE      CONNECTION
--------------------------------------------------------------
ens3    ethernet  connected  Profile 1
lo      loopback  unmanaged  --
</pre>

To delete a connection in nmcli command is as follows:

<pre class=terminal>
nmcli connection delete <uuid>

or

nmcli connection delete id "connection name"
</pre>
