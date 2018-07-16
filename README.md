# Example Playbook

```yaml
---
- name: Prepares and mounts CephFS on a SANBI VM
  hosts: vms
  become: True

  roles:
    - role: ansible-openstack-vm-cephfs
      cephfs_inner_loc: /monitor     # Directory from CephFS to mount to local machine
      cephfs_user: <cephx_user>      # Example user
      cephfs_mountpoint: /mnt        # Where to mount the CephFS directory to on the local machine
      cephfs_accesskey: <cehpx_key>  # User access key
```
