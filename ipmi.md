IPMI
====

```bash
# BMC cold reset
$ IPMICFG -r
```

```bash
# show ipmi info (voltage etc..)
$ IPMICFG -pminfo
```

```bash
# [1282611]
$ ipmitool lan set 1 auth Admin MD5,PASSWORD
$ ipmitool lan set 1 auth Operator MD5,PASSWORD
$ ipmitool lan set 1 auth User MD5,PASSWORD
$ ipmitool lan set 1 auth Callback MD5,PASSWORD
```

```bash
# check user list
$ ipmitool user list 1
# set user name
$ ipmitool user set name 3 ADMIN
# set user password
$ ipmitool user set password 3 ADMIN
$ ipmitool user enable 3
$ ipmitool user priv 3 4 1
```

```bash
$ ipmitool lan print 2
$ ipmitool lan set 2 ipsrc dhcp
$ ipmitool lan set 2 ipsrc static
$ ipmitool lan set 2 ipaddr <ip>
$ ipmitool lan set netmask <netmask>
$ ipmitool lan set 2 defgw ipaddr <defgw>
```

```bash
# show SEL log
$ ipmitool sel list
# clear SEL log
$ ipmitool sel clear
# show real time log
$ ipmitool sdr
# Displays information regarding the high-level status of the system chassis and main power subsystem.
$ ipmitool chassis status
# Show current chassis power status
$ ipmitool chassis power status
# show BMC info
$ ipmitool bmc info
# show channel info
$ ipmitool channel info
```
