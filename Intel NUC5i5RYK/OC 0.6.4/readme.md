{\rtf1\ansi\ansicpg1252\cocoartf2577
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fswiss\fcharset0 Helvetica-Bold;\f1\fswiss\fcharset0 Helvetica;}
{\colortbl;\red255\green255\blue255;\red0\green0\blue0;\red0\green0\blue233;}
{\*\expandedcolortbl;;\cssrgb\c0\c0\c0;\cssrgb\c0\c0\c93333;}
\paperw11900\paperh16840\margl1440\margr1440\vieww11520\viewh8400\viewkind0
\deftab720
\pard\pardeftab720\partightenfactor0

\f0\b\fs50 \cf0 \expnd0\expndtw0\kerning0
Laptop: (5th Gen) Broadwell OpenCore 0.6.4
\f1\b0\fs32 \
\pard\pardeftab720\partightenfactor0
{\field{\*\fldinst{HYPERLINK "https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/broadwell.html"}}{\fldrslt \cf3 \ul \ulc3 https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/broadwell.html}}\
\
\
\pard\pardeftab720\partightenfactor0

\fs60 \cf0 ACPI
\fs32 \
\
\pard\pardeftab720\partightenfactor0

\fs40 \cf0 Add
\fs32 \
\pard\pardeftab720\partightenfactor0

\f0\b \cf0 SSDT-PLUG.aml
\f1\b0  Make sure this file is in your OC/ACPI directory\

\f0\b SSDT-EC.aml
\f1\b0  Make sure this file is in your OC/ACPI directory\
\
\pard\pardeftab720\partightenfactor0

\fs40 \cf0 Delete
\fs32 \
\

\fs40 Patch
\fs32 \
\

\fs40 Quirks
\fs32 \
\pard\pardeftab720\partightenfactor0

\f0\b \cf0 FadtEnableReset
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b NormalizeHeaders
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b RebaseRegions
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b ResetHwSig
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b ResetLogoStatus
\f1\b0  = 
\f0\b No
\f1\b0 \
\
\pard\pardeftab720\partightenfactor0

\fs60 \cf0 Booter
\fs32 \
\
\pard\pardeftab720\partightenfactor0

\fs40 \cf0 MmioWhitelist
\fs32 \
\

\fs40 Patch
\fs32 \
\

\fs40 Quirks
\fs32 \
\pard\pardeftab720\partightenfactor0

\f0\b \cf0 AllowRelocationBlock
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b AvoidRuntimeDefrag
\f1\b0  = 
\f0\b Yes
\f1\b0 \

\f0\b DevirtualiseMmio
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b DisableSingleUser
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b DisableVariableWrite
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b DiscardHibernateMap
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b EnableSafeModeSlide
\f1\b0  = 
\f0\b Yes
\f1\b0 \

\f0\b EnableWriteUnprotector
\f1\b0  = 
\f0\b Yes
\f1\b0 \

\f0\b ForceExitBootServices
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b ProtectMemoryRegions
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b ProtectSecureBoot
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b ProtectUefiServices
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b ProvideCustomSlide
\f1\b0  = 
\f0\b Yes
\f1\b0 \

\f0\b ProvideMaxSlide
\f1\b0  = 
\f0\b 0
\f1\b0 \

\f0\b RebuildAppleMemoryMap
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b SetupVirtualMap
\f1\b0  = 
\f0\b Yes
\f1\b0 \

\f0\b SignalAppleOS
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b SyncRuntimePermissions
\f1\b0  = 
\f0\b No
\f1\b0 \
\
\pard\pardeftab720\partightenfactor0

\fs60 \cf0 DeviceProperties
\fs32 \
\
\pard\pardeftab720\partightenfactor0

\fs40 \cf0 Add
\fs32 \
\pard\pardeftab720\partightenfactor0

\f0\b \cf0 AAPL,ig-platform-id
\f1\b0  = 
\f0\b 02001616
\f1\b0  iGPU set correctly\
\
\pard\pardeftab720\partightenfactor0

\fs40 \cf0 Delete
\fs32 \
\
\pard\pardeftab720\partightenfactor0

\fs60 \cf0 Kernel
\fs32 \
\
\pard\pardeftab720\partightenfactor0

\fs40 \cf0 Add
\fs32 \
\pard\pardeftab720\partightenfactor0

\f0\b \cf0 Lilu.kext
\f1\b0  make sure this Kext is in your 
\f0\b OC/Kexts
\f1\b0  directory and the first kext listed here\

\f0\b Display-2a59-215.kext
\f1\b0  make sure this Kext is in your 
\f0\b OC/Kexts
\f1\b0  directory\

\f0\b AirportItlwm.kext
\f1\b0  make sure this Kext is in your 
\f0\b OC/Kexts
\f1\b0  directory\

\f0\b VirtualSMC.kext
\f1\b0  make sure this Kext is in your 
\f0\b OC/Kexts
\f1\b0  directory\

\f0\b WhateverGreen.kext
\f1\b0  make sure this Kext is in your 
\f0\b OC/Kexts
\f1\b0  directory\

\f0\b AppleALC.kext
\f1\b0  make sure this Kext is in your 
\f0\b OC/Kexts
\f1\b0  directory\

\f0\b IntelMausiEthernet.kext
\f1\b0  make sure this Kext is in your 
\f0\b OC/Kexts
\f1\b0  directory\

\f0\b NVMeFix.kext
\f1\b0  make sure this Kext is in your 
\f0\b OC/Kexts
\f1\b0  directory\

\f0\b SMCProcessor.kext
\f1\b0  make sure this Kext is in your 
\f0\b OC/Kexts
\f1\b0  directory\

\f0\b SMCSuperIO.kext
\f1\b0  make sure this Kext is in your 
\f0\b OC/Kexts
\f1\b0  directory\

\f0\b USBInjectAll.kext
\f1\b0  make sure this Kext is in your 
\f0\b OC/Kexts
\f1\b0  directory\

\f0\b AirportBrcmFixup.kext
\f1\b0  make sure this Kext is in your 
\f0\b OC/Kexts
\f1\b0  directory\

\f0\b AirportBrcmFixup.kext/Contents/PlugIns/AirPortBrcm4360_Injector.kext
\f1\b0  make sure this Kext is in your 
\f0\b OC/Kexts
\f1\b0  directory\

\f0\b AirportBrcmFixup.kext/Contents/PlugIns/AirPortBrcmNIC_Injector.kext
\f1\b0  make sure this Kext is in your 
\f0\b OC/Kexts
\f1\b0  directory\

\f0\b CPUFriend.kext
\f1\b0  make sure this Kext is in your 
\f0\b OC/Kexts
\f1\b0  directory\
\
\pard\pardeftab720\partightenfactor0

\fs40 \cf0 Block
\fs32 \
\

\fs40 Emulate
\fs32 \
\pard\pardeftab720\partightenfactor0

\f0\b \cf0 DummyPowerManagement
\f1\b0  = 
\f0\b No
\f1\b0 \
\
\pard\pardeftab720\partightenfactor0

\fs40 \cf0 Force
\fs32 \
\

\fs40 Patch
\fs32 \
\

\fs40 Quirks
\fs32 \
\pard\pardeftab720\partightenfactor0

\f0\b \cf0 AppleCpuPmCfgLock
\f1\b0  = 
\f0\b Yes
\f1\b0  You should disable if you don't plan to boot 10.10 or older\

\f0\b AppleXcpmCfgLock
\f1\b0  = 
\f0\b Yes
\f1\b0  You should disable CFG-Lock in your bios instead of using this\

\f0\b AppleXcpmExtraMsrs
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b AppleXcpmForceBoost
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b CustomSMBIOSGuid
\f1\b0  = 
\f0\b No
\f1\b0  If you have a Dell or VIAO motherboard, please enable this\

\f0\b DisableIoMapper
\f1\b0  = 
\f0\b Yes
\f1\b0 \

\f0\b DisableRtcChecksum
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b ExtendBTFeatureFlags
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b LegacyCommpage
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b ExternalDiskIcons
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b ForceSecureBootScheme
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b IncreasePciBarSize
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b LapicKernelPanic
\f1\b0  = 
\f0\b No
\f1\b0  If you have an HP laptop, please enable this\

\f0\b PanicNoKextDump
\f1\b0  = 
\f0\b Yes
\f1\b0 \

\f0\b PowerTimeoutKernelPanic
\f1\b0  = 
\f0\b Yes
\f1\b0 \

\f0\b ThirdPartyDrives
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b XhciPortLimit
\f1\b0  = 
\f0\b Yes
\f1\b0  turn off after USB port mapping\
\
\pard\pardeftab720\partightenfactor0

\fs40 \cf0 Scheme
\fs32 \
\
\pard\pardeftab720\partightenfactor0

\fs60 \cf0 Misc
\fs32 \
\
\pard\pardeftab720\partightenfactor0

\fs40 \cf0 BlessOverride
\fs32 \
\

\fs40 Boot
\fs32 \
\pard\pardeftab720\partightenfactor0

\f0\b \cf0 ConsoleAttributes
\f1\b0  = 
\f0\b 0
\f1\b0 \

\f0\b PollAppleHotKeys
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b ShowPicker
\f1\b0  = 
\f0\b Yes
\f1\b0 \

\f0\b TakeoffDelay
\f1\b0  = 
\f0\b 0
\f1\b0 \

\f0\b HibernateMode
\f1\b0  = 
\f0\b None
\f1\b0 \

\f0\b PickerMode
\f1\b0  = 
\f0\b External
\f1\b0  but should normally be 
\f0\b Builtin
\f1\b0 \

\f0\b HideAuxiliary
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b PickerAttributes
\f1\b0  = 
\f0\b 1
\f1\b0 \

\f0\b PickerAudioAssist
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b Timeout
\f1\b0  = 
\f0\b 5
\f1\b0 \
\
\pard\pardeftab720\partightenfactor0

\fs40 \cf0 Debug
\fs32 \
\pard\pardeftab720\partightenfactor0

\f0\b \cf0 AppleDebug
\f1\b0  = 
\f0\b Yes
\f1\b0 \

\f0\b ApplePanic
\f1\b0  = 
\f0\b Yes
\f1\b0 \

\f0\b DisableWatchDog
\f1\b0  = 
\f0\b Yes
\f1\b0 \

\f0\b Target
\f1\b0  = 
\f0\b 67
\f1\b0 \

\f0\b DisplayLevel
\f1\b0  see {\field{\*\fldinst{HYPERLINK "https://dortania.github.io/OpenCore-Install-Guide/troubleshooting/debug.html"}}{\fldrslt \cf3 \ul \ulc3 [Debugging Docs]}} for more info debug display levels\

\f0\b DisplayDelay
\f1\b0  = 
\f0\b 0
\f1\b0 \
\
\pard\pardeftab720\partightenfactor0

\fs40 \cf0 Entries
\fs32 \
\

\fs40 Security
\fs32 \
\pard\pardeftab720\partightenfactor0

\f0\b \cf0 AllowNvramReset
\f1\b0  = 
\f0\b Yes
\f1\b0 \

\f0\b AllowSetDefault
\f1\b0  = 
\f0\b Yes
\f1\b0 \

\f0\b ApECID
\f1\b0  = 
\f0\b 0
\f1\b0 \

\f0\b AuthRestart
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b BlacklistAppleUpdate
\f1\b0  = 
\f0\b Yes
\f1\b0 \

\f0\b BootProtect
\f1\b0  = 
\f0\b None
\f1\b0 \

\f0\b DmgLoading
\f1\b0  = 
\f0\b Signed
\f1\b0 \

\f0\b EnablePassword
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b Vault
\f1\b0  = 
\f0\b Optional
\f1\b0 \

\f0\b SecureBootModel
\f1\b0  = 
\f0\b Default
\f1\b0  SecureBootModel set correctly\

\f0\b HaltLevel
\f1\b0  = 
\f0\b 2147483648
\f1\b0 \

\f0\b ExposeSensitiveData
\f1\b0  = 
\f0\b 6
\f1\b0 \

\f0\b ScanPolicy
\f1\b0  = 
\f0\b 0
\f1\b0 \
\
\pard\pardeftab720\partightenfactor0

\fs40 \cf0 Tools
\fs32 \
You can remove the tool EFIs here\
\
\pard\pardeftab720\partightenfactor0

\fs60 \cf0 NVRAM
\fs32 \
\pard\pardeftab720\partightenfactor0

\f0\b \cf0 LegacyEnable
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b LegacyOverwrite
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b WriteFlash
\f1\b0  = 
\f0\b Yes
\f1\b0 \
\
\pard\pardeftab720\partightenfactor0

\fs40 \cf0 Add
\fs32 \
\pard\pardeftab720\partightenfactor0

\f0\b \cf0 UIScale
\f1\b0  = 
\f0\b 01
\f1\b0 \

\f0\b DefaultBackgroundColor
\f1\b0  = 
\f0\b 00000000
\f1\b0 \

\f0\b boot-args
\f1\b0  = 
\f0\b keepsyms=1 debug=0x100 alcid=1
\f1\b0 \

\f0\b csr-active-config
\f1\b0  = 
\f0\b 00000000
\f1\b0 \

\f0\b prev-lang:kbd
\f1\b0  = 
\f0\b 656e2d55533a30 (en-US:0)
\f1\b0 \

\f0\b SystemAudioVolume
\f1\b0  = 
\f0\b 46
\f1\b0 \
\
\pard\pardeftab720\partightenfactor0

\fs40 \cf0 Delete
\fs32 \
\

\fs40 LegacySchema
\fs32 \
\
\pard\pardeftab720\partightenfactor0

\fs60 \cf0 PlatformInfo
\fs32 \
\pard\pardeftab720\partightenfactor0

\f0\b \cf0 Automatic
\f1\b0  = 
\f0\b Yes
\f1\b0 \

\f0\b UpdateDataHub
\f1\b0  = 
\f0\b Yes
\f1\b0 \

\f0\b UpdateNVRAM
\f1\b0  = 
\f0\b Yes
\f1\b0 \

\f0\b UpdateSMBIOS
\f1\b0  = 
\f0\b Yes
\f1\b0 \

\f0\b UpdateSMBIOSMode
\f1\b0  = 
\f0\b Create
\f1\b0  If you have a Dell or VIAO motherboard, please set this to 
\f0\b Custom
\f1\b0 \
\
\pard\pardeftab720\partightenfactor0

\fs40 \cf0 CustomMemory
\fs32 \
\

\fs40 DataHub
\fs32 \
\

\fs40 Generic
\fs32 \
\pard\pardeftab720\partightenfactor0

\f0\b \cf0 SpoofVendor
\f1\b0  = 
\f0\b Yes
\f1\b0 \

\f0\b AdviseWindows
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b ProcessorType
\f1\b0  = 
\f0\b 1542
\f1\b0 \

\f0\b SystemMemoryStatus
\f1\b0  = 
\f0\b Auto
\f1\b0 \

\f0\b SystemProductName
\f1\b0  = 
\f0\b iMac16,1
\f1\b0 \

\f0\b MLB
\f1\b0  is set\

\f0\b ROM
\f1\b0  is set\

\f0\b SystemSerialNumber
\f1\b0  is set\

\f0\b SystemUUID
\f1\b0  is set\
\
\pard\pardeftab720\partightenfactor0

\fs60 \cf0 UEFI
\fs32 \
\pard\pardeftab720\partightenfactor0

\f0\b \cf0 ConnectDrivers
\f1\b0  = 
\f0\b Yes
\f1\b0 \
\
\pard\pardeftab720\partightenfactor0

\fs40 \cf0 Drivers
\fs32 \
\pard\pardeftab720\partightenfactor0

\f0\b \cf0 HfsPlus.efi
\f1\b0 \

\f0\b OpenRuntime.efi
\f1\b0 \

\f0\b OpenCanopy.efi
\f1\b0 \
\
\pard\pardeftab720\partightenfactor0

\fs40 \cf0 APFS
\fs32 \
\pard\pardeftab720\partightenfactor0

\f0\b \cf0 EnableJumpstart
\f1\b0  = 
\f0\b Yes
\f1\b0 \

\f0\b GlobalConnect
\f1\b0  = 
\f0\b No
\f1\b0  If you have an HP motherboard and can't see APFS drives in OpenCore, please enable this\

\f0\b HideVerbose
\f1\b0  = 
\f0\b Yes
\f1\b0 \

\f0\b JumpstartHotPlug
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b MinDate
\f1\b0  = 
\f0\b 0
\f1\b0 \

\f0\b MinVersion
\f1\b0  = 
\f0\b 0
\f1\b0 \
\
\pard\pardeftab720\partightenfactor0

\fs40 \cf0 Audio
\fs32 \
\pard\pardeftab720\partightenfactor0

\f0\b \cf0 AudioSupport
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b AudioDevice
\f1\b0  = 
\f0\b PciRoot(0x0)/Pci(0x1b,0x0)
\f1\b0 \

\f0\b AudioCodec
\f1\b0  = 
\f0\b 0
\f1\b0 \

\f0\b AudioOut
\f1\b0  = 
\f0\b 0
\f1\b0 \

\f0\b MinimumVolume
\f1\b0  = 
\f0\b 20
\f1\b0 \

\f0\b PlayChime
\f1\b0  = 
\f0\b _-blank-_
\f1\b0 \

\f0\b VolumeAmplifier
\f1\b0  = 
\f0\b 0
\f1\b0 \
\
\pard\pardeftab720\partightenfactor0

\fs40 \cf0 Input
\fs32 \
\pard\pardeftab720\partightenfactor0

\f0\b \cf0 KeyFiltering
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b KeyForgetThreshold
\f1\b0  = 
\f0\b 5
\f1\b0 \

\f0\b KeyMergeThreshold
\f1\b0  = 
\f0\b 2
\f1\b0 \

\f0\b KeySupport
\f1\b0  = 
\f0\b Yes
\f1\b0 \

\f0\b KeySupportMode
\f1\b0  = 
\f0\b Auto
\f1\b0 \

\f0\b KeySwap
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b PointerSupport
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b PointerSupportMode
\f1\b0  = 
\f0\b ASUS
\f1\b0 \

\f0\b TimerResolution
\f1\b0  = 
\f0\b 50000
\f1\b0 \
\
\pard\pardeftab720\partightenfactor0

\fs40 \cf0 Output
\fs32 \
\pard\pardeftab720\partightenfactor0

\f0\b \cf0 TextRenderer
\f1\b0  = 
\f0\b BuiltinGraphics
\f1\b0 \

\f0\b ConsoleMode
\f1\b0  = 
\f0\b _-blank-_
\f1\b0 \

\f0\b Resolution
\f1\b0  = 
\f0\b Max
\f1\b0 \

\f0\b ForceResolution
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b ClearScreenOnModeSwitch
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b IgnoreTextInGraphics
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b ProvideConsoleGop
\f1\b0  = 
\f0\b Yes
\f1\b0 \

\f0\b DirectGopRendering
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b ReconnectOnResChange
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b ReplaceTabWithSpace
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b SanitiseClearScreen
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b UgaPassThrough
\f1\b0  = 
\f0\b No
\f1\b0 \
\
\pard\pardeftab720\partightenfactor0

\fs40 \cf0 ProtocolOverrides
\fs32 \
\pard\pardeftab720\partightenfactor0

\f0\b \cf0 AppleAudio
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b AppleBootPolicy
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b AppleDebugLog
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b AppleEvent
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b AppleFramebufferInfo
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b AppleImageConversion
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b AppleImg4Verification
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b AppleKeyMap
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b AppleRtcRam
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b AppleSecureBoot
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b AppleSmcIo
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b AppleUserInterfaceTheme
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b DataHub
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b DeviceProperties
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b FirmwareVolume
\f1\b0  = 
\f0\b No
\f1\b0  If you plan to use FileVault2, please enable this\

\f0\b HashServices
\f1\b0  = 
\f0\b No
\f1\b0  If you plan to use FileVault2, please enable this\

\f0\b OSInfo
\f1\b0  = 
\f0\b No
\f1\b0 \

\f0\b UnicodeCollation
\f1\b0  = 
\f0\b No
\f1\b0 \
\
\pard\pardeftab720\partightenfactor0

\fs40 \cf0 Quirks
\fs32 \
\pard\pardeftab720\partightenfactor0

\f0\b \cf0 DeduplicateBootOrder
\f1\b0  = 
\f0\b Yes
\f1\b0 \

\f0\b ExitBootServicesDelay
\f1\b0  = 
\f0\b 0
\f1\b0 \

\f0\b IgnoreInvalidFlexRatio
\f1\b0  = 
\f0\b Yes
\f1\b0 \

\f0\b ReleaseUsbOwnership
\f1\b0  = 
\f0\b Yes
\f1\b0 \

\f0\b RequestBootVarRouting
\f1\b0  = 
\f0\b Yes
\f1\b0 \

\f0\b TscSyncTimeout
\f1\b0  = 
\f0\b 0
\f1\b0 \

\f0\b UnblockFsConnect
\f1\b0  = 
\f0\b No
\f1\b0  If you have an HP system, please enable this\
\
\pard\pardeftab720\partightenfactor0

\fs40 \cf0 ReservedMemory}