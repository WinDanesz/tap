"# tap" 

#### reload / start iscsi
systemctl enable/disable iscsid iscsi


#### discover shared partitions
```iscsiadm -m discovery -t sendtargets -p IP ADDRESS:3260```
 
#### auto connect to all stuff
```iscsiadm -m node -L all```

## Setup LVM
```pvcreate /dev/sda```

#### Create a volume group
```vgcreate {size, optional} nameofgroup /firstVolume /secondVolume ...```

#### get a list of the existing volume groups
```vgs```
