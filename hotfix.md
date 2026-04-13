# Update grub


```bash
# /etc/default/grub
GRUB_CMDLINE_LINUX_DEFAULT="quiet splash systemd.unified_cgroup_hierarchy=1 cgroup_no_v1=all"
```

```bash
# update grub config
sudo update-grub
```

Reboot the master node.
