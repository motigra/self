# Home Server

_Documenting my process figuring out how to set up a home server that meets my automation needs, using old hardware where possible_

## Requirements

1. Serve as local NAS, mainly for media storage (photos, videos, music, code)
2. Serve as a backup server, backing up data on both local RAID (or equivalent) as well as external drives
3. Serve as a development/web server capable of running [docker](https://www.docker.com/), VMs, and so on
4. Run Octoprint to manage 3d printer remotely

Additionally, would be nice to have:

5. Ability to run PiHole and other utility software usually deployed standalone
6. Use as media/streaming server to stream media to TV and other devices
7. Use to manage smart home devices, if any
8. Use for IT purposes like deployment/recovery/update management on home PC
9. Use as cache for assets like NPM packages, Steam games etc. on demand (eg. to prepare for a LAN party)
10. Offload computational tasks like rendering/encoding video from main PC

## Design

### Operating System

The options I'm considering are:

 - [TrueNAS](https://www.truenas.com/): Free, based on FreeBSD, uses ZFS
 - UNRAID: One time purchase, linux
 - Ubuntu: Free, linux, requires separate RAID/NAS solution
 - Proxmox: Free (?), debian-linux, not sure if good fit?

Things to consider:

 - Can it run docker?
 - Can it run VMs with linux/windows/other OS?
 - Does it have built-in NAS capabilities?
 - Security
 - Does it support automation?

### Software I'd like to run

 - Docker
 - Home Assistant
 - Plex

## Inventory

TBD

## TO DO

- Design
  - [x] Requirements
  - [ ] Figure out which OS to use
  - [ ] Define HW specs
  - [ ] Do I need ECC memory?
  - [ ] Security and protection
  - [ ] Permandent IP?
  - [ ] Running OctoPrint
  - [ ] Do I need additional HW for PCIe/SATA/USB?
  - [ ] Backups to external drives: snapshots, copy, RAID?
  - [ ] Is it possible to control Zigbee devices with no hub?
- Inventory
  - [ ]  2x old PCs
  - [ ]  Extra/spare hardware
- Purchases
  - [ ]  Additional storage
  - [ ]  Ethernet cable

## Resources

### Videos

 - [Setting up a home server with ubunto - SMB, Plex etc.](https://www.youtube.com/watch?v=72D3MvPk3Xs&ab_channel=HardwareHaven)
 - [Plex media server on pc/unraid - LTT](https://www.youtube.com/watch?v=XKDSld-CrHU&ab_channel=LinusTechTips)
 - [Building an unraid NAS server - LTT](https://www.youtube.com/watch?v=FAy9N1vX76o&ab_channel=LinusTechTips)
 - [Windows-based home server on old hardware - LTT](https://www.youtube.com/watch?v=zPmqbtKwtgw&ab_channel=LinusTechTips)
 - [Home server software & automation with Ansible, Ubuntu](https://www.youtube.com/watch?v=f5jNJDaztqk&ab_channel=Wolfgang%27sChannel)

### Articles

 - ...