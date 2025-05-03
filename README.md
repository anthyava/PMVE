A standalone installation of Home Assistant Core refers to a setup where the Home Assistant Core software is installed directly on a device or operating system, without the use of Docker containers. This provides a simpler, but less flexible and scalable solution, as the software is tightly coupled with the underlying system.

If the LXC is created Privileged, the script will automatically set up USB passthrough.
Use Ubuntu 24.04 ONLY
Requires PVE 8.2.2 with kernel 6.8.4-3-pve or newer
To create a new Proxmox VE Home Assistant Core LXC, run the command below in the Proxmox VE Shell.
To Update, Install HACS or Filebrowser, run the command below (or type update) in the LXC Console.

bash -c "$(wget -qLO - https://github.com/tteck/Proxmox/raw/main/ct/homeassistant-core.sh)"

⚡ Default Settings: 1GB RAM - 8GB Storage - 2vCPU ⚡
Home Assistant Interface: IP:8123

⚙️ Path to HA /config

Copy
/root/.homeassistant
