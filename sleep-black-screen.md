After returning from sleep the laptop screen may be black with a frozen cursor, and terminal inaccessible. To fix that, you can follow those steps:
- https://wiki.archlinux.org/title/Dell_XPS_15_9570#Suspend
- https://www.youtube.com/watch?v=f-u7Zk_itUU (Video format)

In summary:
- Find the GRUB_CMDLINE_LINUX_DEFAULT key at /etc/default/grub
- Append `mem_sleep_default=deep`
- Run `grub-mkconfig -o /boot/grub/grub.cfg`
- Reboot
