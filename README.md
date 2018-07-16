# Example Playbook

```yaml
---
- name: Prepares and mounts CephFS on a SANBI VM
  hosts: vms
  become: True

  roles:
    - role: vm-cephfs
      cephfs_user: <cephx_username> 
      cephfs_mountpoint: /mnt
      cephfs_accesskey: <cehpx_key>
```
