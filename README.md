# server_scripts

Collection of personal scripts that are "server side", meaning that I use to manage/run stuff in my server(s).

## Initial installation

Just a reminder of stuff for the initial installation of an **Arch Linux** installation:

* Follow general [AL installation guide](https://wiki.archlinux.org/index.php/installation_guide).
* Initial packages with pacstrap (really doesn't matter much): `base base-devel linux linux-firmware grub neovim git networkmanager ufw openssh man-db man-pages`
* Configure [grub](https://wiki.archlinux.org/index.php/GRUB) (for a vultr vps: `grub-install --target=i386-pc /dev/vda` and `grub-mkconfig -o /boot/grub/grub.cfg` after chroot'ed).
* Add "normal" user and configure (local) ssh to connect to server with this user and (maybe) root.
* Configure ssh (`/etc/ssh/sshd_config`) and sudoers (`/etc/sudoers`) files.

Once all of the above is already done, I can just execute any script.

## Scripts

General list of scripts already done and ready to use:

- [ ] Nginx webserver.
- [ ] VPN with OpenVPN.
	- [ ] Manage ovpn config files.
- [ ] Email server.
- [ ] Git server.
