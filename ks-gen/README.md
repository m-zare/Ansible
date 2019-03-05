# RHEL Base distribution kickstart generator

These playbook can be used to generate ks.cfg file for automated installation.
Network settings, Partitioning and packages can be managed by using the play.


# Variables

**Redhat and CentOS, 6 and 7:**
```
ks_path
distro
network_list:
- mac_address: mng_mac
  ip
  netmask
  gateway
  dns
- mac_address: srv_mac
  ip
  netmask
  gateway
  dns
hostname
password
partitioning_type
fs_type
swap_size
root_size
u01
pkgs
uefi
home
```
