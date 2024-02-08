# rpi-template

A custom.toml skeleton for Raspberry Pi first boot

## Steps

1. Update custom.toml with appropriate values
2. ```# mount /dev/sd?1 /mnt # Mount the first partition from the RPi image after dd it to disk```
3. ```# cp -f custom.toml /mnt # Copy the updated .toml file for first boot```
4. ```# umount /mnt # Sync and unmount the /boot partition for first boot```
5. Start the host and find its DHCP address from DHCP server

## Reference

On the second partition of the RPi image, a script exists from
the Raspberry Pi foundation: /usr/lib/raspberrypi-sys-mods/init_config
