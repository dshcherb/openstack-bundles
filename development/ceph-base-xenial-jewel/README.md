# Basic Ceph Cluster

This example bundle deploys a basic Ceph cluster (Jewel release) on Ubuntu 16.04 LTS.

## Requirements

This example bundle is designed to run on bare metal using [Juju][] (2.1 or later) with [MAAS][] (Metal-as-a-Service) (2.1 or later); you will need to have setup a [MAAS][] deployment with a minimum of 5 physical servers prior to using this bundle.

Certain configuration options within the bundle may need to be adjusted prior to deployment to fit your particular set of hardware. For example, block device names can vary, passwords should be yours, and machine count may need to be adjusted.

Servers should have:

 - A minimum of 8GB of physical RAM.
 - Enough CPU cores to support your capacity requirements.
 - At least two disks (identified by /dev/sda and /dev/sdb); the first is used by MAAS for the OS install, the second for Ceph storage.

## References

 - OpenStack Dashboard: http://openstack-dashboard_ip/horizon

[MAAS]: https://docs.ubuntu.com/maas
[Juju]: https://jujucharms.com/docs
