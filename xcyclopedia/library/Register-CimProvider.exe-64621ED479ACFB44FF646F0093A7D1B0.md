﻿
# Register-CimProvider.exe 
* File Path: `C:\Windows\SysWOW64\Register-CimProvider.exe`
* Description: WMI
* Comments: 

## Hashes
Type | Hash
-- | --
MD5 | `64621ED479ACFB44FF646F0093A7D1B0`
SHA1 | `1C81416F56A09764AE7FFBEC755DC8A038937B0A`
SHA256 | `08F6185DC43040BABF0219914F4AF40A0AE18B53F3F979F0C1F729D599644270`
SHA384 | `FEB0758E31585F4B9B8C54DF70C061D08F7ED949AB8F8DBD036BCE9052C54F44A5B3C3189EBDF2F80807A51E3F780422`
SHA415 | `4DB5A1B1D8B94D270A97C25E19A25708822D276413EB030E55FCDD6B88F9FEAC4A29385A0A1A8B88A712A72A0C0B44FCA06B1F6091F3A4993E884F4C85C9FB55`
SSDEEP | `384:Hx9lNApeJptUSCMdM+hui/XVKY4gAbNvHettl0rx3Wx1Wf1:LIyvJ5y+huiduNvettlOxOa1`

## Runtime Data
### Usage (stdout):
```Batchfile

Registers CIM Provider into system

Usage:  Register-CimProvider.exe
		-Namespace <NamespaceName>
		-ProviderName <ProviderName>
		-Path <ProviderDllPath>
		[-ClassList <Space delimited list of white-listed classes>]
		[-Impersonation <True or False>]
		[-Decoupled <SDDL>]
		[-HostingModel <HostingModel>]
		[-Localize <locale>]
		[-NoAutorecover]
		[-SupportWQL]
		[-GenerateUnregistration]
		[-ForceUpdate]
		[-Verbose]

-Namespace <NamespaceName>
	Specifies the target namespace of the provider.

-ProviderName <ProviderName>
	Specifies the provider name.

-Path <ProviderDllPath>
	Specifies the provider binary path.

-Impersonation <True or False>
	Specifies foldidentity of decoupled provider, by default is True.

-Decoupled <SDDL>
	Registers provider as decoupled and specifies the security descriptor
	that determines the set of users that can successfully register
	the provider.

-HostingModel <HostingModel>
	Specifies the HostingModel of coupled provider.

-Localize <locale>
	Localizes the provider with resource of specified locale.

-NoAutorecover
	Doesn't autorecover the provider.

-SupportWQL
	Passes the query expression to the filter.

-GenerateUnregistration
	Generate the uninstall mof for the registration,
	which is disabled by default.

-ForceUpdate
	Force update the class if it exists in the system.

-ClassList <ProviderDllPath>
	Specifies space delimited list of white-listed classes that
	will be generated in the mof.

-Verbose
	Outputs registration log.


```

### Usage (stderr):
```Batchfile

```

### Child Processes:


## Signature

* Status: Signature verified.
* Serial: 33000000BCE120FDD27CC8EE930000000000BC
* Thumbprint: E85459B23C232DB3CB94C7A56D47678F58E8E51E
* Issuer: CN=Microsoft Windows Production PCA 2011, O=Microsoft Corporation, L=Redmond, S=Washington, C=US
* Subject: CN=Microsoft Windows, O=Microsoft Corporation, L=Redmond, S=Washington, C=US

## File Metadata

* Original Filename: Register-CimProvider2.exe.mui
* Product Name: Microsoft Windows Operating System
* Company Name: Microsoft Corporation
* File Version: 10.0.14393.0 (rs1_release.160715-1616)
* Product Version: 10.0.14393.0
* Language: English (United States)
* Legal Copyright:  Microsoft Corporation. All rights reserved.

