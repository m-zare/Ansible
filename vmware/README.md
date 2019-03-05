# Variables

**folder-creation:**
```
vcenter_hostname
vcenter_username
vcenter_password
datacenter
folder_type
parent_folder
vm_folder
```
`folder_type: vm, host, datastore, network`

**host-ntp:**
```
vcenter_hostname
vcenter_username
vcenter_password
cluster_name
```

**pg-creation:**
```
cluster_name
vcenter_hostname
esxi_host
vcenter_username
vcenter_password
project_name
portgroup:
- vlan_id
  usage
  dswitch_name
```
`usage: WEB, M-WEB, APP, M-APP, DB, M-DB, DCP`

**vm-creation:**
```
vcenter_hostname
vcenter_username
vcenter_password
datacenter
cluster_name
parent_folder
vm_folder
machine_id
os
distro
machine_usage
project_name
guest_id
datastore_name
disk_size
memory_size
cpu
cpu_per_soc
portgroup:
#manage
- vlan_id
  usage
  dswitch_name
  type
  ip
  netmask
  gateway
#service
- vlan_id
  usage
  dswitch_name
  type
  ip
  netmask
  gateway
iso_datastore
iso_name
```
`guest_id: centos64Guest`

`cpu value should be multiple of num_cpus`

`usage: WEB, M-WEB, APP, M-APP, DB, M-DB, DCP`

**vm-facts:**
```
vcenter_hostname
vcenter_username
vcenter_password
datacenter
machine_name
```

**vm-state:**
```
vcenter_hostname
vcenter_username
vcenter_password
cluster_name
machine_name
status
```