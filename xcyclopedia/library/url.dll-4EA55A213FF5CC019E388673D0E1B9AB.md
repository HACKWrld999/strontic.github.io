﻿---
title: url.dll | Internet Shortcut Shell Extension DLL
excerpt: What is url.dll?
---

# url.dll 

* File Path: `C:\Windows\SysWOW64\url.dll`
* Description: Internet Shortcut Shell Extension DLL

## Hashes

Type | Hash
-- | --
MD5 | `4EA55A213FF5CC019E388673D0E1B9AB`
SHA1 | `D5B0957095904C3E720A8FDF004B3276FDD21A4A`
SHA256 | `CC85A7B90AFBBF967C99F7CB1737E9AD0C7924B03859E4D569C903E2D403A24C`
SHA384 | `2B828982AC824BE20F1961B885F524440CE2E5D1982F41AF0F35483E3B0FB43024E964311AD3D6E882CED3D4E139E97E`
SHA512 | `7BC118736BB2E63161B01D49C7325565411B7A04690145A0B7D2FDE308E1DCDFD0F5412A7A895768A249DE0F61CD19CF4ABCE19289705F34123F319E41F9A6C7`
SSDEEP | `6144:eOM7MMHMMMyMMMZMMMVcRMebzDq0DKF/2Ar++X:eZMMHMMMyMMMZMMMVcR9bzOco2ArZX`
IMP | `CD6DCE6AF077C201EF139C776DCD644F`
PESHA1 | `EFA246A72E8D90423AFAC76D030FEED047D3B173`
PE256 | `2F66E096475C934D1FA4D1E696D41D7AF93092F6B2C2211FCA6AA9B57FF4D22F`

## DLL Exports:

Function Name | Ordinal | Type | Address | Relative Address
-- | -- | -- | -- | --
`AddMIMEFileTypesPS` | 102 (0x66) | Exported Function | 0x632819e0 | 0x000019e0
`TranslateURLW` | 116 (0x74) | Exported Function | 0x632819a0 | 0x000019a0
`TranslateURLA` | 115 (0x73) | Exported Function | 0x63281980 | 0x00001980
`TelnetProtocolHandlerA` | 114 (0x72) | Exported Function | 0x63281740 | 0x00001740
`TelnetProtocolHandler` | 113 (0x71) | Exported Function | 0x63281740 | 0x00001740
`Ordinal101` | 101 (0x65) | Exported Function | 0x632814d0 | 0x000014d0
`OpenURLA` | 112 (0x70) | Exported Function | 0x63281a60 | 0x00001a60
`OpenURL` | 111 (0x6f) | Exported Function | 0x63281a60 | 0x00001a60
`MIMEAssociationDialogW` | 108 (0x6c) | Exported Function | 0x632819c0 | 0x000019c0
`MIMEAssociationDialogA` | 107 (0x6b) | Exported Function | 0x632819c0 | 0x000019c0
`MailToProtocolHandlerA` | 110 (0x6e) | Exported Function | 0x632815a0 | 0x000015a0
`MailToProtocolHandler` | 109 (0x6d) | Exported Function | 0x632815a0 | 0x000015a0
`InetIsOffline` | 106 (0x6a) | Exported Function | 0x63281490 | 0x00001490
`FileProtocolHandlerA` | 105 (0x69) | Exported Function | 0x63281530 | 0x00001530
`FileProtocolHandler` | 104 (0x68) | Exported Function | 0x63281530 | 0x00001530
`AutodialHookCallback` | 103 (0x67) | Exported Function | 0x63281520 | 0x00001520
`URLAssociationDialogA` | 117 (0x75) | Exported Function | 0x632819c0 | 0x000019c0
`URLAssociationDialogW` | 118 (0x76) | Exported Function | 0x632819c0 | 0x000019c0


## Signature

* Status: Signature verified.
* Serial: `3300000266BD1580EFA75CD6D3000000000266`
* Thumbprint: `A4341B9FD50FB9964283220A36A1EF6F6FAA7840`
* Issuer: CN=Microsoft Windows Production PCA 2011, O=Microsoft Corporation, L=Redmond, S=Washington, C=US
* Subject: CN=Microsoft Windows, O=Microsoft Corporation, L=Redmond, S=Washington, C=US

## File Metadata

* Original Filename: URL.DLL
* Product Name: Internet Explorer
* Company Name: Microsoft Corporation
* File Version: 11.00.19041.1 (WinBuild.160101.0800)
* Product Version: 11.00.19041.1
* Language: English (United States)
* Legal Copyright:  Microsoft Corporation. All rights reserved.
* Machine Type: 32-bit

## File Scan

* VirusTotal Detections: 0/70
* VirusTotal Link: https://www.virustotal.com/gui/file/cc85a7b90afbbf967c99f7cb1737e9ad0c7924b03859e4d569c903e2d403a24c/detection/

## File Similarity (ssdeep match)

File | Score
-- | --
[C:\Windows\system32\url.dll](url.dll-3B193173A517524600C63D60FE3C0771.md) | 96

## Possible Misuse

*The following table contains possible examples of `url.dll` being misused. While `url.dll` is **not** inherently malicious, its legitimate functionality can by abused for malicious purposes.*

Source | Source File | Example | License
-- | -- | -- | --
[sigma](https://github.com/Neo23x0/sigma) | [win_susp_rundll32_activity.yml](https://github.com/Neo23x0/sigma/blob/master/rules/windows/process_creation/win_susp_rundll32_activity.yml) | `- '*\rundll32.exe* url.dll,*OpenURL *'` | [DRL 1.0](https://github.com/Neo23x0/sigma/blob/master/LICENSE.Detection.Rules.md)
[sigma](https://github.com/Neo23x0/sigma) | [win_susp_rundll32_activity.yml](https://github.com/Neo23x0/sigma/blob/master/rules/windows/process_creation/win_susp_rundll32_activity.yml) | `- '*\rundll32.exe* url.dll,*OpenURLA *'` | [DRL 1.0](https://github.com/Neo23x0/sigma/blob/master/LICENSE.Detection.Rules.md)
[sigma](https://github.com/Neo23x0/sigma) | [win_susp_rundll32_activity.yml](https://github.com/Neo23x0/sigma/blob/master/rules/windows/process_creation/win_susp_rundll32_activity.yml) | `- '*\rundll32.exe* url.dll,*FileProtocolHandler *'` | [DRL 1.0](https://github.com/Neo23x0/sigma/blob/master/LICENSE.Detection.Rules.md)
[sigma](https://github.com/Neo23x0/sigma) | [win_susp_rundll32_activity.yml](https://github.com/Neo23x0/sigma/blob/master/rules/windows/process_creation/win_susp_rundll32_activity.yml) | `- '* url.dll,*OpenURL *'` | [DRL 1.0](https://github.com/Neo23x0/sigma/blob/master/LICENSE.Detection.Rules.md)
[sigma](https://github.com/Neo23x0/sigma) | [win_susp_rundll32_activity.yml](https://github.com/Neo23x0/sigma/blob/master/rules/windows/process_creation/win_susp_rundll32_activity.yml) | `- '* url.dll,*OpenURLA *'` | [DRL 1.0](https://github.com/Neo23x0/sigma/blob/master/LICENSE.Detection.Rules.md)
[sigma](https://github.com/Neo23x0/sigma) | [win_susp_rundll32_activity.yml](https://github.com/Neo23x0/sigma/blob/master/rules/windows/process_creation/win_susp_rundll32_activity.yml) | `- '* url.dll,*FileProtocolHandler *'` | [DRL 1.0](https://github.com/Neo23x0/sigma/blob/master/LICENSE.Detection.Rules.md)
[LOLBAS](https://github.com/LOLBAS-Project/LOLBAS) | [Url.yml](https://github.com/LOLBAS-Project/LOLBAS/blob/master/yml/OSLibraries/Url.yml) | `Name: Url.dll` | 
[LOLBAS](https://github.com/LOLBAS-Project/LOLBAS) | [Url.yml](https://github.com/LOLBAS-Project/LOLBAS/blob/master/yml/OSLibraries/Url.yml) | `- Command: rundll32.exe url.dll,OpenURL "C:\test\calc.hta"` | 
[LOLBAS](https://github.com/LOLBAS-Project/LOLBAS) | [Url.yml](https://github.com/LOLBAS-Project/LOLBAS/blob/master/yml/OSLibraries/Url.yml) | `- Command: rundll32.exe url.dll,OpenURL "C:\test\calc.url"` | 
[LOLBAS](https://github.com/LOLBAS-Project/LOLBAS) | [Url.yml](https://github.com/LOLBAS-Project/LOLBAS/blob/master/yml/OSLibraries/Url.yml) | `- Command: rundll32.exe url.dll,OpenURL file://^C^:^/^W^i^n^d^o^w^s^/^s^y^s^t^e^m^3^2^/^c^a^l^c^.^e^x^e` | 
[LOLBAS](https://github.com/LOLBAS-Project/LOLBAS) | [Url.yml](https://github.com/LOLBAS-Project/LOLBAS/blob/master/yml/OSLibraries/Url.yml) | `- Command: rundll32.exe url.dll,FileProtocolHandler calc.exe` | 
[LOLBAS](https://github.com/LOLBAS-Project/LOLBAS) | [Url.yml](https://github.com/LOLBAS-Project/LOLBAS/blob/master/yml/OSLibraries/Url.yml) | `- Command: rundll32.exe url.dll,FileProtocolHandler file://^C^:^/^W^i^n^d^o^w^s^/^s^y^s^t^e^m^3^2^/^c^a^l^c^.^e^x^e` | 
[LOLBAS](https://github.com/LOLBAS-Project/LOLBAS) | [Url.yml](https://github.com/LOLBAS-Project/LOLBAS/blob/master/yml/OSLibraries/Url.yml) | `- Command: rundll32.exe url.dll,FileProtocolHandler file:///C:/test/test.hta` | 
[LOLBAS](https://github.com/LOLBAS-Project/LOLBAS) | [Url.yml](https://github.com/LOLBAS-Project/LOLBAS/blob/master/yml/OSLibraries/Url.yml) | `- Path: c:\windows\system32\url.dll` | 
[LOLBAS](https://github.com/LOLBAS-Project/LOLBAS) | [Url.yml](https://github.com/LOLBAS-Project/LOLBAS/blob/master/yml/OSLibraries/Url.yml) | `- Path: c:\windows\syswow64\url.dll` | 
[LOLBAS](https://github.com/LOLBAS-Project/LOLBAS) | [Url.yml](https://github.com/LOLBAS-Project/LOLBAS/blob/master/yml/OSLibraries/Url.yml) | `- Link: https://windows10dll.nirsoft.net/url_dll.html` | 



MIT License. Copyright (c) 2020 Strontic.

