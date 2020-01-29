# Base Centos 7 Packer Build

Requirements:

- vshpere-iso builder is required. 

    - Download the correct version for you OS from [here](https://github.com/jetbrains-infra/packer-builder-vsphere/releases)

## Variable File Format

```yaml
    "vsphere_host": "<IP or HOSTNAME>",
    "vsphere_user": "<Username>",
    "vsphere_pass": "<Password>",
    "insecure_con": "true",
    "esxi_host": "<IP or HOSTNAME>",
    "vsphere_datastore": "<DATASTORE>",
    "vsphere_cluster": "<CLUSTER>",
    "vsphere_folder": "/packer", 
    "ssh_user": "<Username>",
    "ssh_pass": "<Password>",
    "cpus": "2",
    "ram":  "4096",
    "disk_size": "1000000",
    "network": "<Portgroup Name>",

    "iso_loc": "<PATH/TO/ISO",
    "iso_checksum_type": "MD5",
    "iso_checksum": "<CHECKSUM>",
    "floppy_dirs": "files"
```