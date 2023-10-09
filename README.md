# audio-config
The configuration for audio I found in a system that uses archinstall. The systemd services have OpenRC alternative for people that use that.

Instructions:

Move the pipewire folder to /usr/share/

For openrc:
Move the openrc files to /etc/init.d/{WHATEVER_NAME_YOU_CHOOSE}
They need to be seperate.

For systemd(ew)
Move the socket service file to ~/.config/systemd/user/sockets.target.wants/ for the socket file.
Mpve the pipewire service file to ~/.config/systemd/user/default.target.wants/
