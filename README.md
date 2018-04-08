Nordvpn for OpenRC
==================

Introduction
------------

`nordvpn` is a command line helper script to use nordvpn.com for
systems with `openvpn` and `systemd`.
It was created for OpenRC-based Artix Linux but should run without
too much difficulty on systems that satisfy the following dependency list:
- openvpn,
- OpenRC,
- curl,
- unzip,
- ping,
- vpnfailsafe.

Quickstart
----------

- Once installed, run `sudo nordvpn update` to download and install the
configuration files.
- Edit `/etc/openvpn/client/nordvpn/credentials.conf`.
- Run `sudo nordvpn list` to choose a server (alternatively the `rank`
command pings the servers).
- Finally `sudo nordvpn start <servername>`.
- The status command shows you the status of the systemd service.
- See `sudo nordvpn -h` for more information.
