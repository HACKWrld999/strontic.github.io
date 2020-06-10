﻿
# bootcfg.exe 
* File Path: `C:\WINDOWS\SysWOW64\bootcfg.exe`
* Description: BootCfg - Lists or changes the boot settings.
* Comments: 

## Hashes
Type | Hash
-- | --
MD5 | `525D81865EA759DE5C819130AD21F307`
SHA1 | `9AB99D0BE41EACC7EB66B8E35AE6C1831072864E`
SHA256 | `1081A7ACB71B4B984501BEAF35A12DB49B320C4411D65C9B73112DBB3D2AB65E`
SHA384 | `103D71ACCD4C203268669E31F5C2EA89C87250AC463AB4636E343F3195C23D384DC5EA43FBC72C3AD5F4926FDEF2A968`
SHA415 | `BEB1979B8962FAE6914FA8F90D810018891468968D68FFF9BDBC47B136D610DF813C8FC012E14FAACF315A4D79D9BADE6F36AB42BE4AD713ADCF8BDBE4CD34B3`
SSDEEP | `1536:B5QeIGSf5hSuxpzx8m1jue8TR7BpZ0mpmf/hNlGPTykLFa+pdqk:hIGSRhRpzx8mX8TRtpZOblGPT5LFa+Hq`

## Runtime Data
### Usage (stdout):
```Batchfile

BOOTCFG /parameter [arguments]

Description:
    This command line tool can be used to configure, query, change or 
    delete the boot entry settings in the BOOT.INI file.

Parameter List:
    /Copy       Makes a copy of an existing boot entry.

    /Delete     Deletes an existing boot entry from the BOOT.INI file.

    /Query      Displays the current boot entries and their settings.

    /Raw        Allows the user to specify any switch to be added.

    /Timeout    Allows the user to change the Timeout value.

    /Default    Allows the user to change the Default boot entry.

    /EMS        Allows the user to configure the /redirect switch
                for headless support.

    /Debug      Allows the user to specify the port and baudrate for 
                remote debugging.

    /Addsw      Allows the user to add predefined switches.

    /Rmsw       Allows the user to remove predefined switches.

    /Dbg1394    Allows the user to configure 1394 port for debugging.

    /?          Displays this help message.

Examples:
    BOOTCFG /Copy /?
    BOOTCFG /Delete /?
    BOOTCFG /Query /?
    BOOTCFG /Raw /?
    BOOTCFG /Timeout /?
    BOOTCFG /EMS /?
    BOOTCFG /Debug /?
    BOOTCFG /Addsw /?
    BOOTCFG /Rmsw /?
    BOOTCFG /Dbg1394 /?
    BOOTCFG /Default /?
    BOOTCFG /?

WARNING: BOOT.INI is used for boot options on Windows XP and earlier
         operating systems.  Use the BCDEDIT command line tool to modify
         Windows Vista boot options.

```

### Usage (stderr):
```Batchfile
ERROR: Invalid syntax.
Type "BOOTCFG /?" for usage.

```

### Child Processes:


## Signature

* Status: Signature verified.
* Serial: 330000023241FB59996DCC4DFF000000000232
* Thumbprint: FF82BC38E1DA5E596DF374C53E3617F7EDA36B06
* Issuer: CN=Microsoft Windows Production PCA 2011, O=Microsoft Corporation, L=Redmond, S=Washington, C=US
* Subject: CN=Microsoft Windows, O=Microsoft Corporation, L=Redmond, S=Washington, C=US

## File Metadata

* Original Filename: bootcfg.exe.mui
* Product Name: Microsoft Windows Operating System
* Company Name: Microsoft Corporation
* File Version: 10.0.18362.1 (WinBuild.160101.0800)
* Product Version: 10.0.18362.1
* Language: English (United States)
* Legal Copyright:  Microsoft Corporation. All rights reserved.

