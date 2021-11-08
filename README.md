<figure class="table">
            <div class="table-responsive">
              <table><tbody><tr><td colspan="2"><h2>Cisco Basic CLI Commands</h2></td></tr><tr><td><h3><strong>Command&nbsp;</strong></h3></td><td><h3><strong>Purpose</strong></h3></td></tr><tr><td><strong>enable</strong></td><td>Logs you into enable mode, which is also known as user exec mode or privileged mode</td></tr><tr><td><strong>configure terminal</strong></td><td>Logs you into configuration mode</td></tr><tr><td><strong>interface&nbsp;</strong><i>fastethernet/number</i></td><td>Enters interface configuration mode for the specified fast ethernet interface</td></tr><tr><td><strong>reload</strong></td><td>An exec mode command that reboots a Cisco switch or router</td></tr><tr><td><strong>hostname&nbsp;</strong><i>name</i></td><td>Sets a host name to the current Cisco network device</td></tr><tr><td><strong>copy&nbsp;</strong><i>from-location to-location</i></td><td>An enable mode command that copies files from one file location to another</td></tr><tr><td><strong>copy running-config startup-config</strong></td><td>An enable mode command that saves the active config, replacing the startup config when a Cisco network device initializes</td></tr><tr><td><strong>copy startup-config running-config</strong></td><td>An enable mode command that merges the startup config with the currently active config in RAM</td></tr><tr><td><p><strong>write erase</strong></p><p><strong>erase startup-config</strong></p></td><td>An enable mode command that deletes the startup config</td></tr><tr><td><strong>ip address&nbsp;</strong><i>ip-address mask</i></td><td>Assigns an IP address and a subnet mask</td></tr><tr><td><p><strong>shutdown</strong></p><p><strong>no shutdown</strong></p></td><td>Used in interface configuration mode. “Shutdown” shuts down the interface, while “no shutdown” brings up the interface.</td></tr><tr><td><strong>ip default-gateway&nbsp;</strong><i>ip_address</i></td><td>Sets the default gateway on a Cisco device</td></tr><tr><td><strong>show running-config</strong></td><td>An enable mode command that displays the current configuration</td></tr><tr><td><strong>description&nbsp;</strong><i>name-string</i></td><td>A config interface command to describe or name an interface</td></tr><tr><td><strong>show running-config&nbsp;interface&nbsp;</strong><i>interface slot/number</i></td><td>An enable mode command to display the running configuration for a specific interface</td></tr><tr><td><strong>show ip interface&nbsp;</strong><i>[type number]</i></td><td>Displays the usability status of interfaces that are configured for IP</td></tr><tr><td><strong>ip name-server&nbsp;</strong><i>serverip-1 serverip-2</i></td><td>A configure mode command that sets the IP addresses of DNS servers</td></tr><tr><td colspan="2">&nbsp;</td></tr><tr><td colspan="2"><h2>Troubleshooting Commands</h2></td></tr><tr><td><strong>ping&nbsp;</strong><i>{hostname&nbsp;|&nbsp;system-address} [source&nbsp;source-address]</i></td><td>Used in enable mode to diagnose basic network connectivity</td></tr><tr><td><strong>speed&nbsp;</strong><i>{10 | 100 | 1000 | auto}</i></td><td>An interface mode command that manually sets the speed to the specified value or negotiates it automatically</td></tr><tr><td><strong>duplex&nbsp;</strong><i>{auto | full | half}</i></td><td>An interface mode command that manually sets duplex to half, full or auto</td></tr><tr><td><p><strong>cdp run</strong></p><p><strong>no cdp run</strong></p></td><td>A configuration mode command that enables or disables Cisco Discovery Protocol (CDP) for the device</td></tr><tr><td><strong>show mac address-table</strong></td><td>Displays the MAC address table</td></tr><tr><td><strong>show cdp</strong></td><td>Shows whether CDP is enabled globally</td></tr><tr><td><strong>show cdp neighbors</strong><i>[detail]</i></td><td>Lists summary information about each neighbor connected to this device; the “detail” option lists detailed information about each neighbor</td></tr><tr><td><strong>show interfaces</strong></td><td>Displays detailed information about interface status, settings and counters</td></tr><tr><td><strong>show interface status</strong></td><td>Displays the interface line status</td></tr><tr><td><strong>show interfaces switchport</strong></td><td>Displays a large variety of configuration settings and current operational status, including VLAN trunking details.</td></tr><tr><td><strong>show interfaces trunk</strong></td><td>Lists information about the currently operational trunks and the VLANs supported by those trunks</td></tr><tr><td><p><strong>show vlan</strong></p><p><strong>show vlan brief</strong></p></td><td>Lists each VLAN and all interfaces assigned to that VLAN but does not include trunks</td></tr><tr><td><strong>show vtp status</strong></td><td>Lists the current VTP status, including the current mode</td></tr><tr><td colspan="2">&nbsp;</td></tr><tr><td colspan="2"><h2>Routing and VLAN Commands</h2></td></tr><tr><td><strong>ip route</strong><i>network-number network-mask {ip-address | interface}</i></td><td>Sets a static route in the IP routing table</td></tr><tr><td><strong>router rip</strong></td><td>Enables a Routing Information Protocol (RIP) routing process, which places you in router configuration mode</td></tr><tr><td><strong>network&nbsp;</strong><i>ip-address</i></td><td>In router configuration mode, associates a network with a RIP routing process</td></tr><tr><td><strong>version 2</strong></td><td>In router configuration mode, configures the software to receive and send only RIP version 2 packets</td></tr><tr><td><strong>no auto-summary</strong></td><td>In router configuration mode, disables automatic summarization</td></tr><tr><td><strong>default-information originate</strong></td><td>In router configuration mode, generates a default route into RIP</td></tr><tr><td><strong>passive-interface</strong><i>&nbsp;interface</i></td><td>In router configuration mode, sets only that interface to passive RIP mode. In passive RIP mode, RIP routing updates are accepted by, but not sent out of, the specified interface.</td></tr><tr><td><strong>show ip rip database</strong></td><td>Displays the contents of the RIP routing database</td></tr><tr><td><strong>ip nat&nbsp;</strong><i>[inside&nbsp;|&nbsp;outside]</i></td><td>An interface configuration mode command to designate that traffic originating from or destined for the interface is subject to NAT</td></tr><tr><td><strong>ip nat inside source&nbsp;</strong><i>{list{access-list-number&nbsp;|&nbsp;access-list-name}}&nbsp;interface&nbsp;type number[overload]</i></td><td>A configuration mode command to establish dynamic source translation. Use of the&nbsp;“list”&nbsp;keyword enables you to use an ACL to identify the traffic that will be subject to NAT. The&nbsp;“overload”&nbsp;option enables the router to use one global address for many local addresses.</td></tr><tr><td><strong>ip nat inside source static&nbsp;</strong><i>local-ip global-ip</i></td><td>A configuration mode command to establish a static translation between an inside local address and an inside global address</td></tr><tr><td><strong>vlan</strong></td><td>Creates a VLAN and enters VLAN configuration mode for further definitions</td></tr><tr><td><strong>switchport access vlan</strong></td><td>Sets the VLAN that the interface belongs to.</td></tr><tr><td><strong>switchport trunk encapsulation dot1q</strong></td><td>Specifies 802.1Q encapsulation on the trunk link.</td></tr><tr><td><strong>switchport access</strong></td><td>Assigns this port to a VLAN</td></tr><tr><td><strong>vlan&nbsp;vlan-id&nbsp;</strong><i>[name vlan-name]</i></td><td>Configures a specific VLAN name (1 to 32 characters)</td></tr><tr><td><strong>switchport mode&nbsp;</strong><i>{ access | trunk&nbsp;}</i></td><td>Configures the VLAN membership mode of a port. The access port is set to access unconditionally and operates as a non-trunking, single VLAN interface that sends and receives non-encapsulated (non-tagged) frames. An access port can be assigned to only one VLAN.<br>The trunk port sends and receives encapsulated (tagged) frames that identify the VLAN of origination. A trunk is a point-to-point link between two switches or between a switch and a router.</td></tr><tr><td><strong>switchport trunk&nbsp;</strong><i>{encapsulation { dot1q }</i></td><td>Sets the trunk characteristics when the interface is in trunking mode. In this mode, the switch supports simultaneous tagged and untagged traffic on a port.</td></tr><tr><td><strong>encapsulation dot1q&nbsp;vlan-id</strong></td><td>A configuration mode command that defines the matching criteria to map 802.1Q frames ingress on an interface to the appropriate service instance</td></tr><tr><td colspan="2">&nbsp;</td></tr><tr><td colspan="2"><h2>DHCP Commands</h2></td></tr><tr><td><strong>ip address dhcp</strong></td><td>A configuration mode command to acquire an IP address on an interface via DHCP</td></tr><tr><td><strong>ip dhcp pool&nbsp;name</strong></td><td>A configuration mode command to configure a DHCP address pool on a DHCP server and enter DHCP pool configuration mode</td></tr><tr><td><strong>domain-name&nbsp;</strong><i>domain</i></td><td>Used in DHCP pool configuration mode to specify the domain name for a DHCP client</td></tr><tr><td><strong>network&nbsp;</strong><i>network-number&nbsp;[mask]</i></td><td>Used in DHCP pool configuration mode to configure the network number and mask for a DHCP address pool primary or secondary subnet on a Cisco IOS DHCP server</td></tr><tr><td><strong>ip dhcp excluded-address&nbsp;</strong><i>ip-address&nbsp;[last-ip-address]</i></td><td>A configuration mode command to specify IP addresses that a DHCP server should not assign to DHCP clients</td></tr><tr><td><strong>ip helper-address&nbsp;</strong><i>address</i></td><td>An interface configuration mode command to enable forwarding of UDP broadcasts, including BOOTP, received on an interface</td></tr><tr><td><strong>default-router&nbsp;</strong><i>address[address2 ... address8]</i></td><td>Used in DHCP pool configuration mode to specify the default router list for a DHCP client</td></tr><tr><td colspan="2">&nbsp;</td></tr><tr><td colspan="2"><h2>Security Commands</h2></td></tr><tr><td><strong>password</strong><i>pass-value</i></td><td>Lists the password that is required if the&nbsp;login&nbsp;command (with no other parameters) is conﬁgured</td></tr><tr><td><strong>username&nbsp;</strong><i>name</i><strong>&nbsp;password&nbsp;</strong><i>pass-value</i></td><td>A global command that deﬁnes one of possibly multiple user names and associated passwords used for user authentication. It is used when the&nbsp;login local&nbsp;line conﬁguration command has been used.</td></tr><tr><td><strong>enable password&nbsp;</strong><i>pass-value</i></td><td>A configuration mode command that deﬁnes the password required when using the&nbsp;<strong>enable</strong>&nbsp;command</td></tr><tr><td><strong>enable secret</strong><i>pass-value</i></td><td>A configuration mode command that sets this Cisco device password that is required for any user to enter enable mode</td></tr><tr><td><strong>service password-encryption</strong></td><td>A configuration mode command that directs the Cisco IOS software to encrypt the passwords, CHAP secrets, and similar data saved in its configuration file</td></tr><tr><td><strong>ip domain-name&nbsp;</strong><i>name</i></td><td>Conﬁgures a DNS domain name&nbsp;</td></tr><tr><td><strong>crypto key generate rsa</strong></td><td>A configuration mode command that creates and stores (in a hidden location in ﬂash memory) the keys that are required by SSH</td></tr><tr><td><strong>transport input&nbsp;</strong><i>{telnet | ssh}</i></td><td>Used in vty line conﬁguration mode, deﬁnes whether Telnet or SSH access is allowed into this switch. Both values can be specified in a single command to allow both Telnet and SSH access (default settings).</td></tr><tr><td><strong>access-list&nbsp;</strong><i>access-list-number&nbsp;{deny | permit}&nbsp;source&nbsp;[source-wildcard] [log]</i></td><td>A configuration mode command that defines a standard IP access list</td></tr><tr><td><strong>access-class</strong></td><td>Restricts incoming and outgoing connections between a particular vty (into a basic Cisco device) and the addresses in an access list</td></tr><tr><td><strong>ip access-list&nbsp;</strong><i>{standard&nbsp;|&nbsp;extended} {access-list-name&nbsp;|&nbsp;access-list-number}</i></td><td>A configuration mode command that defines an IP access list by name or number</td></tr><tr><td><strong>permit&nbsp;source&nbsp;</strong><i>[source-wildcard]</i></td><td>Used in ACL configuration mode to set conditions to allow a packet to pass a named IP ACL. To remove a permit condition from an ACL, use the&nbsp;“no”&nbsp;form of this command.</td></tr><tr><td><strong>deny&nbsp;source&nbsp;</strong><i>[source-wildcard]</i></td><td>Used in ACL configuration mode to set conditions in a named IP ACL that will deny packets. To remove a deny condition from an ACL, use the&nbsp;“no”&nbsp;form of this command.</td></tr><tr><td><strong>ntp peer&nbsp;</strong><i>&lt;ip-address&gt;</i></td><td>Used in global configuration mode to configure the software clock to synchronize a peer or to be synchronized by a peer</td></tr><tr><td><strong>switchport port-security</strong></td><td>Used in interface configuration mode to enable port security on the interface</td></tr><tr><td><strong>switchport port-security maximum&nbsp;maximum</strong></td><td>Used in interface configuration mode to set the maximum number of secure MAC addresses on the port</td></tr><tr><td><strong>switchport port-security mac-address&nbsp;</strong><i>{mac-addr&nbsp;| {sticky [mac-addr]}}&nbsp;</i><br><br><br>&nbsp;</td><td>Used in interface configuration mode to add a MAC address to the list of secure MAC addresses. The “sticky” option configures the MAC addresses as sticky on the interface.</td></tr><tr><td><strong>switchport port-security violation&nbsp;</strong><i>{shutdown&nbsp;|&nbsp;restrict&nbsp;|&nbsp;protect}</i></td><td>Used in interface configuration mode to set the action to be taken when a security violation is detected</td></tr><tr><td><strong>show port security&nbsp;</strong><i>[interface interface-id]</i></td><td>Displays information about security options configured on the interface</td></tr><tr><td colspan="2">&nbsp;</td></tr><tr><td colspan="2"><h2>Monitoring and Logging Commands</h2></td></tr><tr><td><strong>logging&nbsp;</strong><i>ip address</i></td><td>Configures the IP address of the host that will receive the system logging (syslog) messages</td></tr><tr><td><strong>logging trap&nbsp;level</strong></td><td>Used in configuration mode to limit messages that are logged to the syslog servers based on severity. Specify the number or name of the desired severity level at which messages should be logged.</td></tr><tr><td><strong>show logging</strong></td><td>Enable mode command that displays the state of system logging (syslog) and the contents of the standard system logging buffer.</td></tr><tr><td><strong>terminal monitor</strong></td><td>An enable mode command that tells Cisco IOS to send a copy of all syslog messages, including debug messages, to the Telnet or SSH user who issues this command</td></tr></tbody></table>
            </div></figure>
