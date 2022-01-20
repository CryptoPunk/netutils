# netutils
scripts to do repetitive network tasks

## create_wlan
```
Usage: create_wlan [OPTION]...
Short description of the software
Mandatory arguments to long options are mandatory for short options too.

  -l, --list-phy	List the available wifi physical layer devices and exit.
  -p, --phy=PHY		Use the wifi physical layer device PHY to create the AP.
			  default: phy0

  -a, --ap=AP		Name the AP network interface AP. 
			  default: ap0

  -s, --ssid=SSID	Use the specified SSID for the AP. 
			  default: TestNet

  -p, --password=PASS	Use password PASS to secure the AP. 
			  default: MonkeyVSRobot

  -R, --redirect=[HOST:]PORT:RHOST:RPORT
			Redirect traffic going to HOST:PORT to RHOST:RPORT.
			If HOST is not specified, all traffic to PORT is 
			redirected to RHOST:RPORT
			
  -C, --cleanup		Run cleanup again, useful if interfaces get left behind
			after exiting uncleanly

  -n, --net=IP/CIDR	Use the IP and CIDR range on the AP network.
			  default: 192.168.77.1/24
  -N, --NAT=IFACE	Use IFACE as the outbound NAT interface
			  default: wlp1s0
      --disable-dns	Disables the DNS server
      --disable-dhcp    Disables the DHCP server
  -v, --verbose		Include debugging output
  -h, --help		This help screen

Examples:

  create_wlan --phy=phy0 --ssid=TestNet --password=Tester

```


