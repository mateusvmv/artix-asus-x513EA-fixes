Fn key locking may not work by default, to fix that install asusctl
`pacman -S asusctl`

To get it to start with openrc you can follow [this discussion](https://gitlab.com/asus-linux/asusctl/-/issues/59)
In summary:
- Get the asusd file found in the files directory of this repository
- Place it in `/etc/init.d/asusd`
- Add asusd to the default group by running `rc-update add asusd`
- Start asusd without a reboot with `rc-service asusd start`
