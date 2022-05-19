# crash
Crash Report
panic(cpu 0 caller 0xffffff7f995fae60): "virtual bool IOAccelLegacyDisplayMachine::display_mode_did_change(uint32_t): AMDRadeonAccelerator driver returns false" @IOAccelLegacyDisplayMachine.cpp:267
Panicked task 0xffffff86ae9bf700: 10 threads: pid 156: WindowServer
Backtrace (CPU 0), panicked thread: 0xffffff99e0a44000, Frame : Return Address
0xffffffd0ec273540 : 0xffffff8000683e2d 
0xffffffd0ec273590 : 0xffffff80007e3cb6 
0xffffffd0ec2735d0 : 0xffffff80007d350d 
0xffffffd0ec273620 : 0xffffff8000623a60 
0xffffffd0ec273640 : 0xffffff80006841fd 
0xffffffd0ec273760 : 0xffffff80006839b6 
0xffffffd0ec2737c0 : 0xffffff8000f164bf 
0xffffffd0ec2738b0 : 0xffffff7f995fae60 
0xffffffd0ec2738c0 : 0xffffff7f995a3a36 
0xffffffd0ec273900 : 0xffffff7f995ecd7b 
0xffffffd0ec273960 : 0xffffff7f9975fbf4 
0xffffffd0ec273aa0 : 0xffffff7f9974a099 
0xffffffd0ec273b30 : 0xffffff7f99755635 
0xffffffd0ec273b50 : 0xffffff7f9975a366 
0xffffffd0ec273be0 : 0xffffff7f813fbda0 
0xffffffd0ec273c10 : 0xffffff7f9974ff0e 
0xffffffd0ec273ca0 : 0xffffff8000e14abc 
0xffffffd0ec273d00 : 0xffffff8000e830db 
0xffffffd0ec273d60 : 0xffffff8000789b97 
0xffffffd0ec273db0 : 0xffffff800068a6db 
0xffffffd0ec273e10 : 0xffffff800065ed03 
0xffffffd0ec273e60 : 0xffffff8000675259 
0xffffffd0ec273ef0 : 0xffffff80007b61a8 
0xffffffd0ec273fa0 : 0xffffff8000624246 
      Kernel Extensions in backtrace:
         com.apple.iokit.IOGraphicsFamily(594.0)[3ECB2385-311A-374E-9C0F-65639BA26A05]@0xffffff7f9973f000->0xffffff7f9976dfff
            dependency: com.apple.iokit.IOPCIFamily(2.9)[A436E92C-DE10-3718-AEF4-ED2A788A466A]@0xffffff8003203000->0xffffff800322efff
         com.apple.iokit.IOAcceleratorFamily2(462.8)[2ED59269-2A13-3F67-AB1A-212DB14FC5F2]@0xffffff7f995a2000->0xffffff7f9960cfff
            dependency: com.apple.driver.AppleMobileFileIntegrity(1.0.5)[2C07C501-6849-3156-ABBF-BBA8477F46E5]@0xffffff8001d91000->0xffffff8001db2fff
            dependency: com.apple.iokit.IOGraphicsFamily(594)[3ECB2385-311A-374E-9C0F-65639BA26A05]@0xffffff7f9973f000->0xffffff7f9976dfff
            dependency: com.apple.iokit.IOPCIFamily(2.9)[A436E92C-DE10-3718-AEF4-ED2A788A466A]@0xffffff8003203000->0xffffff800322efff
            dependency: com.apple.iokit.IOReportFamily(47)[ABB60963-29B6-3098-87E8-41E21DABF443]@0xffffff8003240000->0xffffff8003242fff
            dependency: com.apple.iokit.IOSurface(302.14)[1DA5DCF0-D472-33C0-90C9-2AB910EBC473]@0xffffff8003373000->0xffffff800338ffff
         com.apple.kext.AMDFramebuffer(4.0.8)[2E42215C-251C-3026-B86A-F08139C86E86]@0xffffff7f813fb000->0xffffff7f8141ffff
            dependency: com.apple.iokit.IOACPIFamily(1.4)[CF250EA9-AE5C-3215-BCF5-763DB70A0228]@0xffffff8002d60000->0xffffff8002d61fff
            dependency: com.apple.iokit.IOGraphicsFamily(594)[3ECB2385-311A-374E-9C0F-65639BA26A05]@0xffffff7f9973f000->0xffffff7f9976dfff
            dependency: com.apple.iokit.IOPCIFamily(2.9)[A436E92C-DE10-3718-AEF4-ED2A788A466A]@0xffffff8003203000->0xffffff800322efff
            dependency: com.apple.kext.AMDSupport(4.0.8)[110BBBA3-A511-3F4C-8FDD-935FBEEE2E2A]@0xffffff7f97c25000->0xffffff7f97ceafff

Process name corresponding to current thread (0xffffff99e0a44000): WindowServer

Mac OS version:
21E258

Kernel version:
Darwin Kernel Version 21.4.0: Fri Mar 18 00:45:05 PDT 2022; root:xnu-8020.101.4~15/RELEASE_X86_64
Kernel UUID: B6F8637B-0844-355F-8C82-60FA06149384
KernelCache slide: 0x0000000000400000
KernelCache base:  0xffffff8000600000
Kernel slide:      0x0000000000410000
Kernel text base:  0xffffff8000610000
__HIB  text base: 0xffffff8000500000
System model name: iMac18,2 (Mac-77F17D7DA9285301)
System shutdown begun: NO
Panic diags file available: YES (0x0)
Hibernation exit count: 0

System uptime in nanoseconds: 10207378087
Last Sleep:           absolute           base_tsc          base_nano
  Uptime  : 0x0000000260683d0b
  Sleep   : 0x0000000000000000 0x0000000000000000 0x0000000000000000
  Wake    : 0x0000000000000000 0x0000000670502826 0x0000000000000000
Compressor Info: 0% of compressed pages limit (OK) and 0% of segments limit (OK) with 0 swapfiles and OK swap space
Zone info:
  Foreign : 0xffffff8016e07000 - 0xffffff8016e15000
  Native  : 0xffffff804821b000 - 0xffffffa04821b000
  Readonly: 0xffffff8514ee7000 - 0xffffff86ae880000
  Metadata: 0xffffffe98ded7000 - 0xffffffe9ae1ec000
  Bitmaps : 0xffffffe9ae1ec000 - 0xffffffe9ba1ec000

last started kext at 9499117165: >AudioAUUC	1.70 (addr 0xffffff7f994a9000, size 12288)
loaded kexts:
>AudioAUUC	1.70
>!ATopCaseHIDEventDriver	5440.11
>!APlatformEnabler	2.7.0d0
>X86PlatformShim	1.0.0
>AGPM	127
@filesystems.autofs	3.0
>!AUpstreamUserClient	3.6.9
>!AHDAHardwareConfigDriver	340.2
@kext.AMDFramebuffer	4.0.8
>!AHDA	340.2
@kext.AMDRadeonX4000	4.0.8
@kext.AMDRadeonServiceManager	4.0.8
>!A!IKBLGraphics	18.0.5
>!A!IKBLGraphicsFramebuffer	18.0.5
>!AGraphicsDevicePolicy	6.5.7
>!AGFXHDA	140.3
>eficheck	1
>AGDCBacklightControl	6.5.7
>!ABacklight	180.5
@AGDCPluginDisplayMetrics	6.5.7
>!AMCCSControl	1.15
>pmtelemetry	1
|IOUserEthernet	1.0.1
>usb.!UUserHCI	1
>!AHV	1
>!ADiskImages2	126.100.13
>!ASMCLMU	212
>!AFIVRDriver	4.1.0
>ACPI_SMC_PlatformPlugin	1.0.0
@UVCService	1
>!A!IPCHPMC	2.0.1
@kext.AMD9500!C	4.0.8
>!AThunderboltIP	4.0.3
>!A!ISlowAdaptiveClocking	4.0.0
>!AFileSystemDriver	3.0.1
@filesystems.tmpfs	1
@filesystems.lifs	1
@filesystems.hfs.kext	583.100.10
@BootCache	40
@!AFSCompression.!AFSCompressionTypeZlib	1.0.0
@!AFSCompression.!AFSCompressionTypeDataless	1.0.0d1
@filesystems.apfs	1934.101.3
>!ASDXC	3.2.1
|!ABCM5701Ethernet	11.0.0
>AirPort.BrcmNIC	1400.1.1
>!AAHCIPort	351.100.4
@private.KextAudit	1.0
>!AACPIButtons	6.1
>!ARTC	2.0.1
>!ASMBIOS	2.1
>!AACPIEC	6.1
>!AAPIC	1.7
@!ASystemPolicy	2.0.0
@nke.applicationfirewall	402
|IOKitRegistryCompatibility	1
|EndpointSecurity	1
@Dont_Steal_Mac_OS_X	7.0.0
@kec.!AEncryptedArchive	1
>!AMultitouchDriver	5440.11
>!AInputDeviceSupport	5440.6
>!AHS!BDriver	5440.11
>IO!BHIDDriver	9.0.0
@kext.triggers	1.0
>DspFuncLib	340.2
@kext.OSvKernDSPLib	529
@kext.AMDRadeonX4200HWLibs	1.0
>!UAudio	415.11
>!AAudioClockLibs	140.1
@kext.AMDRadeonX4000HWServices	4.0.8
|IOAccelerator!F2	462.8
>!AGraphicsControl	6.5.7
>!AHDA!C	340.2
|IOHDA!F	340.2
|IOAudio!F	340.2
@vecLib.kext	1.2.0
>!ASMBusPCI	1.0.14d1
>!ABacklightExpert	1.1.0
>!ASMBus!C	1.0.18d1
|IO!BSerialManager	9.0.0
|IO!BPacketLogger	9.0.0
|IO!BHost!CUSBTransport	9.0.0
|IO!BHost!CUARTTransport	9.0.0
|IO!BHost!CTransport	9.0.0
>IO!BHost!CPCIeTransport	9.0.0
|IOAVB!F	1040.6
@plugin.IOgPTPPlugin	1040.3
|IOEthernetAVB!C	1.1.0
|CSR!BHost!CUSBTransport	9.0.0
|Broadcom!BHost!CUSBTransport	9.0.0
|Broadcom!B20703USBTransport	9.0.0
>!AIPAppender	1.0
>IOPlatformPluginLegacy	1.0.0
>X86PlatformPlugin	1.0.0
>IOPlatformPlugin!F	6.0.0d8
|IONDRVSupport	594
@kext.AMDSupport	4.0.8
>!AThunderboltEDMSink	5.0.3
>!AThunderboltDPOutAdapter	8.5.1
@!AGPUWrangler	6.5.7
@!AGraphicsDeviceControl	6.5.7
|IOGraphics!F	594
|IOSlowAdaptiveClocking!F	1.0.0
>usb.IOUSBHostHIDDevice	1.2
>usb.cdc	5.0.0
>usb.networking	5.0.0
>usb.!UHostCompositeDevice	1.2
>!AThunderboltPCIDownAdapter	4.1.1
>!AThunderboltDPInAdapter	8.5.1
>!AThunderboltDPAdapter!F	8.5.1
>!AHPM	3.4.4
>!A!ILpssI2C!C	3.0.60
>!A!ILpssI2C	3.0.60
>!A!ILpssDmac	3.0.60
>!ABSDKextStarter	3
|IOSurface	302.14
@filesystems.hfs.encodings.kext	1
>!AXsanScheme	3
>!AThunderboltNHI	7.2.81
|IOThunderbolt!F	9.3.3
|IONVMe!F	2.1.0
|IO80211!FLegacy	1200.12.2b1
|IOSkywalk!F	1.0
>mDNSOffloadUserClient	1.0.1b8
>corecapture	1.0.4
|IOAHCI!F	297
>!A!ILpssGspi	3.0.60
>usb.!UXHCIPCI	1.2
>usb.!UXHCI	1.2
>usb.!UHostPacketFilter	1.0
|IOUSB!F	900.4.2
>!AEFINVRAM	2.1
>!AEFIRuntime	2.1
|IOSMBus!F	1.1
|IOHID!F	2.0.0
|IOTimeSync!F	1040.3
|IONetworking!F	3.4
>DiskImages	493.0.0
|IO!B!F	9.0.0
|IOReport!F	47
$quarantine	4
$sandbox	300.0
@kext.!AMatch	1.0.0d1
|CoreAnalytics!F	1
>!ASSE	1.0
>!AKeyStore	2
>!UTDM	533.100.11
|IOUSBMass!SDriver	210.101.2
|IOSCSIBlockCommandsDevice	456.100.7
|IO!S!F	2.1
|IOSCSIArchitectureModel!F	456.100.7
>!AMobileFileIntegrity	1.0.5
$!AImage4	4.2.0
@kext.CoreTrust	1
>!AFDEKeyStore	28.30
>!AEffaceable!S	1.0
>!ACredentialManager	1.0
>KernelRelayHost	1
|IOUSBHost!F	1.2
>!UHostMergeProperties	1.2
>usb.!UCommon	1.0
>!ABusPower!C	1.0
>!ASEPManager	1.0.1
>IOSlaveProcessor	1
>!AACPIPlatform	6.1
>!ASMC	3.1.9
|IOPCI!F	2.9
|IOACPI!F	1.4
>watchdog	1
@kec.pthread	1
@kec.Libm	1
@kec.corecrypto	12.0

