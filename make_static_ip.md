# Making static IP :
1) vi /etc/sysconfig/network-scripts/ifcfg-ens192

  TYPE="Ethernet"
  PROXY_METHOD="none"
  BROWSER_ONLY="no"
  BOOTPROTO=none           change
  IPADDR=192.168.1.122     change 
  NETMASK=255.255.255.0    change 
  GATEWAY=192.168.1.1
  DEFROUTE="yes"
  IPV4_FAILURE_FATAL="no"
  IPV6INIT="yes"
  IPV6_AUTOCONF="yes"
  IPV6_DEFROUTE="yes"
  IPV6_FAILURE_FATAL="no"
  IPV6_ADDR_GEN_MODE="stable-privacy"
  NAME="ens192"
  UUID="3d70e36f-d1e1-4064-af24-76129f07e592"
  DEVICE="ens192"
  ONBOOT="yes"

2) systemctl restart network
3) ystemctl status network
