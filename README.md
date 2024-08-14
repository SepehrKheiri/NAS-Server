# Repurposing Old Hardware: NAS (Network Attached Storage)


## Overview
For this short home project I wanted to work with hardware and repurpose an old machine that did not function as something useful on my local network: a NAS. The computer will be able to locally host files at a static IP, and will also be running as a personal media server.




## 1. Hardware

### This computer has had a corrupt drive and been left untouched for 5 years, so I need to first do a few things to the hardware:
- Clean and dust internals, so the air can properly flow.
- Remove old corrupt HDD and install new SSD.
- Disassemble and reapply thermal paste on GPU & CPU.
![IMG_4573](https://github.com/blwhit/NAS-Server/assets/141170960/d53a990a-e01a-4f39-bd2a-dc63b0c3f44b)
![IMG_4574](https://github.com/blwhit/NAS-Server/assets/141170960/9e042c05-53d6-428b-95db-2af307a4b894)
![IMG_4576](https://github.com/blwhit/NAS-Server/assets/141170960/cf426fd0-b4c0-4a58-9ca4-404c99361d9e)
(No SSD Support)
![IMG_4581](https://github.com/blwhit/NAS-Server/assets/141170960/aeb266eb-24ff-4792-a8b4-a4454e0e7bde)



## 2. Software

### Installing Ubuntu, Server config, and Network config:


- The most challenging part of this project was the left-behind artifacts from the corrupted Windows OS that ran on the original drive. 
- The machine will boot to Ubuntu but will not properly install, and is stuck in a loop asking for Windows Bootable Media.
- I fixed this by first clearing the CMOS with a jumper/removing the on-board battery and then changing the Ubuntu version to the LTS (Long Term Support) version.

![image](https://github.com/blwhit/NAS-Server/assets/141170960/6318a8cd-e406-4523-b86f-c495c5c1c1dc)
![image](https://github.com/blwhit/NAS-Server/assets/141170960/f5d84ed3-2675-4fa7-8ec5-3a3dd45b650a)
![IMG_4584](https://github.com/blwhit/NAS-Server/assets/141170960/26480e97-bef1-458f-b8c0-97750aff8ec5)



- Next I wired the computer into my network and gave it a static IP for ease of use.
![Capture000](https://github.com/blwhit/NAS-Server/assets/141170960/f424141e-7e17-491d-bf32-828367ac8ba5)




- Install an OpenSSH server via command-line for secure remote communication.
- Install Plex to run a local Media Server.
- Remote connect to files via WinSCP and access Plex server GUI through local IP in browser
  ![Capture00](https://github.com/blwhit/NAS-Server/assets/141170960/d6ca3322-91a3-4b48-9ffc-ca73b0ecb2ab)

  ![Capturefff](https://github.com/blwhit/NAS-Server/assets/141170960/f83b5d4a-ac47-492b-8ef6-edea65d72da8)
