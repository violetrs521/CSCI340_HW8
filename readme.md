# Homework 8
## Violet Smith
### March 30th

#### 1. Device Information

##### a. Program lsblk
<b> output: </b>
NAME   MAJ:MIN RM   SIZE RO TYPE MOUNTPOINT
loop0    7:0    0 212.1M  1 loop /snap/code/88
loop1    7:1    0     4K  1 loop /snap/bare/5
loop2    7:2    0 209.1M  1 loop /snap/code/91
loop3    7:3    0 110.8M  1 loop /snap/core/12725
loop4    7:4    0 110.7M  1 loop /snap/core/12821
loop5    7:5    0  55.5M  1 loop /snap/core18/2344
loop6    7:6    0  55.5M  1 loop /snap/core18/2284
loop7    7:7    0  61.9M  1 loop /snap/core20/1361
loop8    7:8    0 149.9M  1 loop /snap/gnome-3-28-1804/71
loop9    7:9    0  61.9M  1 loop /snap/core20/1376
loop10   7:10   0  54.2M  1 loop /snap/snap-store/558
loop11   7:11   0  65.2M  1 loop /snap/gtk-common-themes/1519
loop12   7:12   0 247.9M  1 loop /snap/gnome-3-38-2004/87
loop13   7:13   0 164.8M  1 loop /snap/gnome-3-28-1804/161
loop14   7:14   0  44.2M  1 loop /snap/gtk-common-themes/1353
loop15   7:15   0   219M  1 loop /snap/gnome-3-34-1804/77
loop16   7:16   0 248.8M  1 loop /snap/gnome-3-38-2004/99
sda      8:0    0   500G  0 disk 
├─sda1   8:1    0 220.6G  0 part /
├─sda2   8:2    0   954M  0 part /boot
├─sda3   8:3    0   8.4G  0 part [SWAP]
└─sda4   8:4    0 270.1G  0 part /home
sr0     11:0    1  1024M  0 rom  


<b> Column Descriptions: </b>
- Name: Lists the names of the devices
- MAJ:MIN: Major device number : Minor device number
- RM: 0 if the device can not be removed 1 if the device can be removed
- Size: outputs the size of the device
- RO: 1 if the device is read only 0 if the device is not read only
- Type: type of the disk
- MountPoint: the devices mount point

##### b. Program lsusb

<b> Program output:</b>
Bus 001 Device 002: ID 80ee:0021 VirtualBox USB Tablet
Bus 001 Device 001: ID 1d6b:0001 Linux Foundation 1.1 root hub

<b> Column Descriptions: <b>
- The first column shows you the bus number, each bus represent connections to your device
- The second column represents the device number
- The third colom represents the vendor Id : product ID 
- The fourth column represents the vendor name and the product
  
#### Storage Nomenclature

##### a. Host Bus Adapter
  <p> A host bus adapter is a type of circut board. This circut boards connects to a host system to a storage or network device. The purpose of the host bus adapter is that it helps I/O processig reducing the host's microprocessors load when storing and getiing data. This helps improve the overall performace of the host. </p>
  
##### b. Serial ATA(SATA)
   <p> Serial ATA, or Serial AT Attachment (SATA) is a interface that connects host bus adapters to mass storage devices. These mass storage devices can be hard drives, optical drives, etc. Parallel ATA was the device in place, in the 1980's, to do this before Serial ATA came out as a better alternative to it. SATA's are usually used to connect hard disk drives to a host system. The SATA has transfer rates which are much faster than PATA and ATA. The SATA also allows for hot swapping meaning you can replace computer components without shutting off the computer. This was not possible with the PATA. </p>
  
##### c. Fiber Channel
   <p> Fiber Channels are used to transfer large data quickly between one or more computers through interconnected storage servers. This is used usually for storage networking server enviornments as a alternative to small computer system interface.The FC-specific swich is known as the fabric. There is also usually a FC port used to achice FC-based data transfers.  </p>
  
##### d. iSCSI
   <p> Internet Small Computer System Interface or iSCSI is a way of linking data storage facilities through an internet protocol. It is a way of managing storage over long distances. It gives block level access to storage devices. It does this by carrying SCSI commands over a TCP-based IP network. The iSCSI can be used to transmit data over the internet, LAN or WAN and it can enable non location dependent data storage and retrieval. ISCSI doesn't support object storage access or Network attached storage. </p>
  
##### e. Storage Area Network (SAN)
   <p> Storage Area Networks provide block level network access to storage through a high speed network, they are one of the main storage architectures. SAN's are typically used to improve application performance, increase storage effectivness, improve data security, improve application avalibility, and they usually play an important role in an organizations Bussiness community management activities. SAN's provide storage devices to a host so the storage appears locally attached. SAN's are generally based on FC technology. </p>
  
##### f. Network Attached Storage (NAS)
   <p> Network attached storage is used to make stored data more accessible to networked devices. It is a file-level storage architecture. NAS is another of the main storage architectures. It gives a single point to access to networks with security builtin and fault tolerant capabilities. NAS has preconfigured storage hardware such as NAS boxees, NAS units, NAS servers, and NAS heads. NAS allows for better performance, easy setup, fault tolerance, scale out capacity, and accesibility.  </p>
