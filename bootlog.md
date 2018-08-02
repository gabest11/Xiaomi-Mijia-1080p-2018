```
udhcpc: entering released state
ÿ
U-Boot SPL 2013.07 (May 16 2018 - 03:40:21)
pll_init:365
l2cache_clk = 375000000
pll_cfg.pdiv = 8, pll_cfg.h2div = 4, pll_cfg.h0div = 4, pll_cfg.cdiv = 1, pll_cfg.l2div = 2
nf=30 nr = 1 od0 = 1 od1 = 1
cppcr is 03c05100
CPM_CPAPCR 03b0890d
nf=42 nr = 1 od0 = 1 od1 = 1
cppcr is 02a04900
CPM_CPMPCR 07d0c90d
nf=50 nr = 1 od0 = 1 od1 = 1
cppcr is 03204900
CPM_CPVPCR 0320490d
cppcr 0x9a794410
apll_freq 712704000 
mpll_freq 1000000000 
vpll_freq = 1200000000
ddr sel mpll, cpu sel apll
ddrfreq 500000000
cclk  712704000
l2clk 356352000
h0clk 250000000
h2clk 250000000
pclk  125000000
DDRC_DLP:0000f003


U-Boot 2013.07 (May 16 2018 - 03:40:21)

Board: ISVP (Ingenic XBurst T20 SoC)
DRAM:  64 MiB
Top of RAM usable for U-Boot at: 84000000
Reserving 422k for U-Boot at: 83f94000
Reserving 32784k for malloc() at: 81f90000
Reserving 32 Bytes for Board Info at: 81f8ffe0
Reserving 124 Bytes for Global Data at: 81f8ff64
Reserving 128k for boot params() at: 81f6ff64
Stack Pointer at: 81f6ff48
Now running in RAM - U-Boot at: 83f94000
MMC:   msc: 0
the manufacturer ef
SF: Detected W25Q128

*** Warning - bad CRC, using default environment

In:    serial
Out:   serial
Err:   serial
start tf recovery detect ...
read file start
reading tf_recovery.img
** Unable to read file tf_recovery.img **
read file size -1 
data check start
Invalid data len
data check NG
the manufacturer ef
SF: Detected W25Q128

--->probe spend 4 ms
SF: 2621440 bytes @ 0x40000 Read: OK
--->read spend 339 ms
## Booting kernel from Legacy Image at 80600000 ...
   Image Name:   Linux-3.10.14
   Image Type:   MIPS Linux Kernel Image (gzip compressed)
   Data Size:    2240049 Bytes = 2.1 MiB
   Load Address: 80010000
   Entry Point:  80380060
   Verifying Checksum ... OK
   Uncompressing Kernel Image ... OK

Starting kernel ...

[    0.000000] Initializing cgroup subsys cpu
[    0.000000] Initializing cgroup subsys cpuacct
[    0.000000] Linux version 3.10.14 (jenkins@64bf91150a4e) (gcc version 4.7.2 (Ingenic r2.3.3 2016.12) ) #1 PREEMPT Sat Jun 30 07:40:49 UTC 2018
[    0.000000] bootconsole [early0] enabled
[    0.000000] CPU0 RESET ERROR PC:C9A65E32
[    0.000000] CPU0 revision is: 00d00101 (Ingenic Xburst)
[    0.000000] FPU revision is: 00b70000
[    0.000000] CCLK:712MHz L2CLK:356Mhz H0CLK:200MHz H2CLK:200Mhz PCLK:100Mhz
[    0.000000] Determined physical RAM map:
[    0.000000]  memory: 0049e000 @ 00010000 (usable)
[    0.000000]  memory: 00032000 @ 004ae000 (usable after init)
[    0.000000] User-defined physical RAM map:
[    0.000000]  memory: 02880000 @ 00000000 (usable)
[    0.000000] Zone ranges:
[    0.000000]   Normal   [mem 0x00000000-0x0287ffff]
[    0.000000] Movable zone start for each node
[    0.000000] Early memory node ranges
[    0.000000]   node   0: [mem 0x00000000-0x0287ffff]
[    0.000000] Primary instruction cache 32kB, 8-way, VIPT, linesize 32 bytes.
[    0.000000] Primary data cache 32kB, 8-way, VIPT, no aliases, linesize 32 bytes
[    0.000000] pls check processor_id[0x00d00101],sc_jz not support!
[    0.000000] MIPS secondary cache 128kB, 8-way, linesize 32 bytes.
[    0.000000] Built 1 zonelists in Zone order, mobility grouping off.  Total pages: 10287
[    0.000000] Kernel command line: console=ttyS1,115200n8 mem=41472K@0x0 ispmem=8M@0x2880000 rmem=15872K@0x3080000 init=/linuxrc rootfstype=squashfs root=/dev/mtdblock2 rw mtdparts=jz_sfc:256k(boot),2560k(kernel),7104k(rootfs),6336k(data),64k(config),64k(factory)
[    0.000000] PID hash table entries: 256 (order: -2, 1024 bytes)
[    0.000000] Dentry cache hash table entries: 8192 (order: 3, 32768 bytes)
[    0.000000] Inode-cache hash table entries: 4096 (order: 2, 16384 bytes)
[    0.000000] Memory: 35460k/41472k available (3552k kernel code, 6012k reserved, 1175k data, 200k init, 0k highmem)
[    0.000000] SLUB: HWalign=32, Order=0-3, MinObjects=0, CPUs=1, Nodes=1
[    0.000000] Preemptible hierarchical RCU implementation.
[    0.000000] NR_IRQS:418
[    0.000000] clockevents_config_and_register success.
[    0.000028] Calibrating delay loop... 709.42 BogoMIPS (lpj=3547136)
[    0.057702] pid_max: default: 32768 minimum: 301
[    0.062746] Mount-cache hash table entries: 512
[    0.067958] Initializing cgroup subsys debug
[    0.072222] Initializing cgroup subsys freezer
[    0.078276] devtmpfs: initialized
[    0.083251] regulator-dummy: no parameters
[    0.087612] NET: Registered protocol family 16
[    0.110949] bio: create slab <bio-0> at 0
[    0.117800] jz-dma jz-dma: JZ SoC DMA initialized
[    0.122905] usbcore: registered new interface driver usbfs
[    0.128545] usbcore: registered new interface driver hub
[    0.134026] usbcore: registered new device driver usb
[    0.139339] i2c-gpio i2c-gpio.1: using pins 57 (SDA) and 58 (SCL)
[    0.145600]  (null): set:249  hold:250 dev=100000000 h=500 l=500
[    0.151719] media: Linux media interface: v0.10
[    0.156310] Linux video capture interface: v2.00
[    0.162352] Switching to clocksource jz_clocksource
[    0.167319] cfg80211: Calling CRDA to update world regulatory domain
[    0.173736] cfg80211: World regulatory domain updated:
[    0.180112] jz-dwc2 jz-dwc2: cgu clk gate get error
[    0.184997] DWC IN DEVICE ONLY MODE
[    0.188582] cfg80211:   (start_freq - end_freq @ bandwidth), (max_antenna_gain, max_eirp)
[    0.197519] dwc2 dwc2: Keep PHY ON
[    0.200929] dwc2 dwc2: Using Buffer DMA mode
[    0.205222] dwc2 dwc2: Core Release: 3.00a
[    0.209391] cfg80211:   (2402000 KHz - 2472000 KHz @ 40000 KHz), (2000 mBi, 0 mBm)
[    0.217049] cfg80211:   (2457000 KHz - 2482000 KHz @ 20000 KHz), (2000 mBi, 0 mBm)
[    0.225090] dwc2 dwc2: enter dwc2_gadget_plug_change:2611: plugin = 1 pullup_on = 0 suspend = 0
[    0.233900] cfg80211:   (2474000 KHz - 2494000 KHz @ 20000 KHz), (2000 mBi, 0 mBm)
[    0.241779] NET: Registered protocol family 2
[    0.246748] TCP established hash table entries: 512 (order: 0, 4096 bytes)
[    0.253732] cfg80211:   (5170000 KHz - 5250000 KHz @ 80000 KHz), (2000 mBi, 0 mBm)
[    0.261389] TCP bind hash table entries: 512 (order: -1, 2048 bytes)
[    0.267798] TCP: Hash tables configured (established 512 bind 512)
[    0.274078] cfg80211:   (5250000 KHz - 5330000 KHz @ 80000 KHz), (2000 mBi, 0 mBm)
[    0.281757] cfg80211:   (5490000 KHz - 5730000 KHz @ 160000 KHz), (2000 mBi, 0 mBm)
[    0.289594] TCP: reno registered
[    0.292795] UDP hash table entries: 256 (order: 0, 4096 bytes)
[    0.298726] UDP-Lite hash table entries: 256 (order: 0, 4096 bytes)
[    0.305102] cfg80211:   (5735000 KHz - 5835000 KHz @ 80000 KHz), (2000 mBi, 0 mBm)
[    0.312766] cfg80211:   (57240000 KHz - 63720000 KHz @ 2160000 KHz), (N/A, 0 mBm)
[    0.320713] NET: Registered protocol family 1
[    0.325507] RPC: Registered named UNIX socket transport module.
[    0.331524] RPC: Registered udp transport module.
[    0.336217] RPC: Registered tcp transport module.
[    0.341003] RPC: Registered tcp NFSv4.1 backchannel transport module.
[    0.348068] freq_udelay_jiffys[0].max_num = 10
[    0.352550] cpufreq 	udelay 	loops_per_jiffy	
[    0.356914] 12000	 59724	 59724	
[    0.360197] 24000	 119448	 119448	
[    0.363623] 60000	 298620	 298620	
[    0.367067] 120000	 597241	 597241	
[    0.370657] 200000	 995402	 995402	
[    0.374130] 300000	 1493103	 1493103	
[    0.377838] 600000	 2986206	 2986206	
[    0.381569] 792000	 3941793	 3941793	
[    0.385255] 1008000	 5016827	 5016827	
[    0.389066] 1200000	 5972413	 5972413	
[    0.399506] squashfs: version 4.0 (2009/01/31) Phillip Lougher
[    0.405582] exFAT: Version 1.2.9
[    0.408880] exFAT: Core Version 1.2.9
[    0.413531] jffs2: version 2.2. © 2001-2006 Red Hat, Inc.
[    0.419606] msgmni has been set to 69
[    0.424928] io scheduler noop registered
[    0.428872] io scheduler cfq registered (default)
[    0.437064] jz-uart.1: ttyS1 at MMIO 0x10031000 (irq = 58) is a uart1
[    0.445722] console [ttyS1] enabled, bootconsole disabled
[    0.445722] console [ttyS1] enabled, bootconsole disabled
[    0.462933] brd: module loaded
[    0.469218] loop: module loaded
[    0.473399] zram: Created 2 device(s) ...
[    0.477682] logger: created 256K log 'log_main'
[    0.483501] jz SADC driver registeres over!
[    0.489680] jz TCU driver register completed
[    0.494594] the id code = ef4018, the flash name is WIN25Q128
[    0.500563] JZ SFC Controller for SFC channel 0 driver register
[    0.506682] 6 cmdlinepart partitions found on MTD device jz_sfc
[    0.512798] Creating 6 MTD partitions on "jz_sfc":
[    0.517738] 0x000000000000-0x000000040000 : "boot"
[    0.523529] 0x000000040000-0x0000002c0000 : "kernel"
[    0.529490] 0x0000002c0000-0x0000009b0000 : "rootfs"
[    0.535384] 0x0000009b0000-0x000000fe0000 : "data"
[    0.541177] 0x000000fe0000-0x000000ff0000 : "config"
[    0.547118] 0x000000ff0000-0x000001000000 : "factory"
[    0.553194] SPI NOR MTD LOAD OK
[    0.556514] tun: Universal TUN/TAP device driver, 1.6
[    0.561764] tun: (C) 1999-2004 Max Krasnyansky <maxk@qualcomm.com>
[    0.568383] wait stable.[246][cgu_macphy]
[    0.572564] Bus Mode Reg after reset: 0x00020101, cnt=0
[    0.578990] Bus Mode Reg after reset: 0x00020101, cnt=1
[    0.585367] Bus Mode Reg after reset: 0x00020101, cnt=2
[    0.591782] Bus Mode Reg after reset: 0x00020101, cnt=3
[    0.598158] Bus Mode Reg after reset: 0x00020101, cnt=4
[    0.604556] Bus Mode Reg after reset: 0x00020101, cnt=5
[    0.610954] Bus Mode Reg after reset: 0x00020101, cnt=6
[    0.617327] Bus Mode Reg after reset: 0x00020101, cnt=7
[    0.623717] Bus Mode Reg after reset: 0x00020101, cnt=8
[    0.630106] Bus Mode Reg after reset: 0x00020101, cnt=9
[    0.636480] func:jz_mii_bus_probe, synopGMAC_reset failed
[    0.642068] jz_mii_bus: probe of jz_mii_bus.0 failed with error -1
[    0.648527] =======>gmacdev = 0x82210d80<================
[    0.654118] =========>gmacdev->MacBase = 0xb34b0000 DmaBase = 0xb34b1000
[    0.661036] Bus Mode Reg after reset: 0x00020101, cnt=0
[    0.667412] Bus Mode Reg after reset: 0x00020101, cnt=1
[    0.673801] Bus Mode Reg after reset: 0x00020101, cnt=2
[    0.680190] Bus Mode Reg after reset: 0x00020101, cnt=3
[    0.686565] Bus Mode Reg after reset: 0x00020101, cnt=4
[    0.692953] Bus Mode Reg after reset: 0x00020101, cnt=5
[    0.699339] Bus Mode Reg after reset: 0x00020101, cnt=6
[    0.705711] Bus Mode Reg after reset: 0x00020101, cnt=7
[    0.712098] Bus Mode Reg after reset: 0x00020101, cnt=8
[    0.718473] Bus Mode Reg after reset: 0x00020101, cnt=9
[    0.724860] func:jz_mac_probe, synopGMAC_reset failed
[    0.730081] jz_mac: probe of jz_mac.0 failed with error -1
[    0.736293] jzmmc_v1.2 jzmmc_v1.2.0: vmmc regulator missing
[    0.748989] jzmmc_v1.2 jzmmc_v1.2.0: card inserted, state=0
[    0.778995] jzmmc_v1.2 jzmmc_v1.2.0: register success!
[    0.784350] jzmmc_v1.2 jzmmc_v1.2.1: vmmc regulator missing
[    0.829105] jzmmc_v1.2 jzmmc_v1.2.1: register success!
[    0.835081] TCP: cubic registered
[    0.838503] NET: Registered protocol family 17
[    0.845561] input: gpio-keys as /devices/platform/gpio-keys/input/input0
[    0.852929] drivers/rtc/hctosys.c: unable to open rtc device (rtc0)
[    0.864839] VFS: Mounted root (squashfs filesystem) readonly on device 31:2.
[    0.877879] devtmpfs: mounted
[    0.881461] Freeing unused kernel memory: 200K (804ae000 - 804e0000)
+ source /etc/hooks/pre-init
+ exec chroot . /bin/busybox linuxrc
[    1.784996] mmc0: SD Status: Invalid Allocation Unit size.
[    1.792654] mmc0: new SD card at address e624
[    1.797580] mmcblk0: mmc0:e624 SU512 483 MiB 
[    1.803650]  mmcblk0: p1
Starting logging: OK
Starting mdev...
+ flock 9
+ destdir=/mnt/sdcard
+ '[' -z mmcblk0 ]
+ my_umount mmcblk0
+ grep -q /mnt/sdcard
+ grep 'mmcblk0 ' /proc/mounts
+ my_mount mmcblk0
+ grep -q ' /mnt/sdcard ' /proc/mounts
+ mount -t auto -odirsync /dev/mmcblk0 /mnt/sdcard
mount: mounting /dev/mmcblk0 on /mnt/sdcard failed: Input/output error
+ exit 1
+ flock 9
+ destdir=/mnt/sdcard
+ '[' -z mmcblk0p1 ]
+ my_umount mmcblk0p1
+ grep -q /mnt/sdcard
+ grep 'mmcblk0p1 ' /proc/mounts
+ my_mount mmcblk0p1
+ grep -q ' /mnt/sdcard ' /proc/mounts
+ mount -t auto -odirsync /dev/mmcblk0p1 /mnt/sdcard
[    2.986448] FAT-fs (mmcblk0p1): Volume was not properly unmounted. Some data may be corrupt. Please run fsck.
Remount sensor config file path to data...
[    3.618437] jz_pwm_probe[210] d_name = tcu_chn2
[    3.666814] request pwm channel 2 successfully
[    3.675203] pwm-jz pwm-jz: jz_pwm_probe register ok !
[    3.862345] register all isp device successfully!
[    3.871450] @@@@ tx-isp-probe ok @@@@@
[    3.906641] jz_codec_register: probe() successful!
[    4.259469] dma dma0chan24: Channel 24 have been requested.(phy id 7,type 0x06 desc a1a07000)
[    4.268758] dma dma0chan25: Channel 25 have been requested.(phy id 6,type 0x06 desc a1a06000)
Starting mdev...
+ flock 9
+ destdir=/mnt/sdcard
+ '[' -z mmcblk0 ]
+ my_umount mmcblk0
+ grep -q /mnt/sdcard
+ grep 'mmcblk0 ' /proc/mounts
+ my_mount mmcblk0
+ grep -q ' /mnt/sdcard ' /proc/mounts
+ exit 1
+ flock 9
+ destdir=/mnt/sdcard
+ '[' -z mmcblk0p1 ]
+ my_umount mmcblk0p1
+ grep -q /mnt/sdcard
+ grep 'mmcblk0p1 ' /proc/mounts
+ umount -l /mnt/sdcard
+ my_mount mmcblk0p1
+ grep -q ' /mnt/sdcard ' /proc/mounts
+ mount -t auto -odirsync /dev/mmcblk0p1 /mnt/sdcard
[    4.470311] FAT-fs (mmcblk0p1): Volume was not properly unmounted. Some data may be corrupt. Please run fsck.
Copy back log in TF
read-only file system detected...done
Starting network: OK
install wlan driver....
[    5.420103] RTL871X: module init start
[    5.423979] RTL871X: rtl8189fs v4.3.24.8_22657.20170607
[    5.432775] RTL871X: build time: Jun 30 2018 07:42:04
[    5.438017] wlan power on
[    5.459522] RTL871X: module init ret=0
Starting wifi ......
[    5.505284] mmc1: card claims to support voltages below the defined range. These will be ignored.
wlan0
[    5.540816] mmc1: new SDIO card at address 0001
[    5.617341] RTL871X: HW EFUSE
[    5.622404] RTL871X: wifi_mac file: /tmp/wifimac.txt
[    5.627597] RTL871X: hal_com_config_channel_plan chplan:0x48
[    5.842494] RTL871X: rtw_regsty_chk_target_tx_power_valid return _FALSE for band:0, path:0, rs:0, t:-1
[    5.871486] RTL871X: rtw_ndev_init(wlan0) if1 mac_addr=7c:49:eb:ab:43:f2
++++ ok
Enabling wifi STA mode
Entering service runlevel normal
******** (SSID removed)
******** (password removed)
WPA
killall: udhcpc: no process killed
­

+±±é wpa_supplicant: no process killed
killall: hostapd: no process killed
killall: udhcpd: no process killed
miio_qrcode: set for deactivation
rescan triggered for deactivation set on 1 service
®¬¹triggered for activation set on 1 service
miio_agent: set for activation
rescan triggered for activation set on 1 service
miio_algo: set for activation
rescan triggered for activation set on 1 service
miio_client: set for activation
rescan triggered for activation set on 1 service
miio_client_helper: set for activation
rescan triggered for activation set on 1 service
miio_cloud: set for activation
rescan triggered for activation set on 1 service
miio_devicekit: set for activation
rescan triggered for activation set on 1 service
miio_nas: set for activation
rescan triggered for activation set on 1 service
miio_ota: set for activation
rescan triggered for activation set on 1 service
miio_record: set for activation
rescan triggered for activation set on 1 service
miio_sdcard: set for activation
rescan triggered for activation set on 1 service
miio_stream: set for activation
rescan triggered for activation set on 1 service
mortox: set for activation
rescan triggered for activation set on 1 service
Starting crond...
Start detecting tf_recovery.img
/mnt/sdcard/tf_recovery.img not exist
Starting netcheck...
[   10.192868] set sensor gpio as PA-low-10bit
[   10.233779] ps5250 0-0048: ps5250 chip found @ 0x48 (i2c0)
[   10.245199] tx_isp: Registered sensor subdevice ps5250 0-0048
[   10.830092] ###### image_tuning_v4l2_open 4329 #######
[   10.997542] &&& chan1  scaler.max_width = 1920 max_height = 1080  min_width = 128 min_height = 128 &&&
[   11.020526] &&& chan2  scaler.max_width = 800 max_height = 800  min_width = 128 min_height = 128 &&&
Successfully initialized wpa_supplicant
[   11.112060] info: drop frame cnt = 1
[   11.212290] info: drop frame cnt = 0
[   11.216555] info: drop frame cnt = 1
[   11.261974] info: drop frame cnt = 0
[   11.458988] codec_set_device: set device: MIC...
[   11.719059] codec_set_device: set device: speaker...
rfkill: Cannot open RFKILL control device
nl80211: Could not re-add multicast membership for vendor events: -2 (No such file or directory)
mijia_camera_v3
udhcpc: started, v1.28.1
udhcpc: sending discover
udhcpc: sending discover
udhcpc: sending discover
```