<h1> My Homelab</h1>

<p>My homelab currently consists of the following:</p>
<li>Mini PC</li>

- Said Mini PC is a Dell OptiPlex 7040m, it's got an i5 6500T @ 2.50Ghz, 32GB of DDR4 Memory and 1TB base storage (split into 1x2.5" 500GB SSD & 1xM.2 NVME 500GB SSD). <br>
- Rather than use this PC as a bare metal machine, I've turned it into a hypervisor using VMware ESXi 7, this has allowed me to create multiple virtual machines to run various services and applications all on one consolidated machine. <br>
- At this moment in time I've got the following virtual machines/services/applications running on it:<br>
  - Jumpbox, so I can remotely connect to my home network. [Windows]<br>
  - Docker running VaultWarden for my Password Manager and Caddy as a Certificate Authority for my local services (such as VaultWarden & Adguard). [Ubuntu]<br>
  - Adguard Home to block ads and tracking. [Ubuntu]<br>
  - Minecraft server for me and my friendt to play on. [Ubuntu Server]<br>
  - Plex server to host media content for myself, family & friends to watch on. [Ubuntu]<br>
  - CheckMK to monitor all of the aforementioned VMs and any other device that can be monitored (My main PC, NAS, Network Switch, etc). [Ubuntu]<br>

<li>NAS Server</li>

- The NAS (Network Attached Storage) server I'm using right now is the Synology DS918+, I've got 4x4TB NAS HDDs plugged in for a total of 16TB storage, with RAID 5 (my selected RAID configuration) that becomes a usable total of 11TB.<br>
- Alongside the hard drives, I have 2 M.2 NVMe SSDs installed to provide with read/write cache to increase the speed and performance of reading & writing data to the NAS.
- I mainly use my NAS as a form of backup for any kind of data such as projects, videos, music, documents, etc, on top of this I have it attached as a network drive to my Plex server so all my media content that I want to watch it stored on the NAS, as opposed to storing locally on the mini PC, in turn saving space for future VMs.<br>

<li>Network Switch</li>

- The Network Switch I use is an 8-Port Cisco switch, this is what connects my homelab devices together and most importantly, connects them all to the router for internet connectivity.<br>
