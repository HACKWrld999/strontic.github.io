﻿---
title: ktpass.exe | Kerberos keytab tool
excerpt: What is ktpass.exe?
---

# ktpass.exe 

* File Path: `C:\windows\system32\ktpass.exe`
* Description: Kerberos keytab tool

## Hashes

Type | Hash
-- | --
MD5 | `1EA55F7524824B824958EA9A1F49BDAA`
SHA1 | `0B8B59C65BD8AC468E5F4A0C5B7367472C359DF9`
SHA256 | `AEB6E5BA6A6FAEB9ACDC989C7E7177D8800EE21B5539C88885B3392C37D61E3D`
SHA384 | `815632FECA1A855D3ED875FBBBEE6AC362668C9261C7A8870DFFF28B9DB5925CA68DDA4F7E680A7FCAC799D5FBD93740`
SHA512 | `9FA81A6C4DC6934BE9ECB4C956E41C5432F09365A91759EE8A66543C2F5FFB9FC05EAED93766EB9DAB6619A001DE6A080D98C5664EC4DFC3D5D11A5F9E5555A9`
SSDEEP | `768:t0wqYYvnLjHIIM/ZpDKX3eK+FvNcGCZs3I24hvJZ+pQbEY3r/rAXQeEb:t0fnHIIM3Ke/FAB42nbzjb`

## Signature

* Status: The file C:\windows\system32\ktpass.exe is not digitally signed. You cannot run this script on the current system. For more information about running scripts and setting execution policy, see about_Execution_Policies at http://go.microsoft.com/fwlink/?LinkID=135170
* Serial: ``
* Thumbprint: ``
* Issuer: 
* Subject: 

## File Metadata

* Original Filename: ktpass.exe.mui
* Product Name: Microsoft Windows Operating System
* Company Name: Microsoft Corporation
* File Version: 6.3.9600.16384 (winblue_rtm.130821-1623)
* Product Version: 6.3.9600.16384
* Language: English (United States)
* Legal Copyright:  Microsoft Corporation. All rights reserved.




## Additional Info*

**The information below is copied from [MicrosoftDocs](https://github.com/MicrosoftDocs/windowsserverdocs), which is maintained by [Microsoft](https://opensource.microsoft.com/codeofconduct/). Available under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) license.*

---

## ktpass

> Applies to: Windows Server (Semi-Annual Channel), Windows Server 2019, Windows Server 2016, Windows Server 2012 R2, Windows Server 2012

Configures the server principal name for the host or service in Active Directory Domain Services (AD DS) and generates a .keytab file that contains the shared secret key of the service. The .keytab file is based on the Massachusetts Institute of Technology (MIT) implementation of the Kerberos authentication protocol. The ktpass command-line tool allows non-Windows services that support Kerberos authentication to use the interoperability features provided by the Kerberos Key Distribution Center (KDC) service.

### Syntax

```
ktpass
[/out <filename>]
[/princ <principalname>]
[/mapuser <useraccount>]
[/mapop {add|set}] [{-|+}desonly] [/in <filename>]
[/pass {password|*|{-|+}rndpass}]
[/minpass]
[/maxpass]
[/crypto {DES-CBC-CRC|DES-CBC-MD5|RC4-HMAC-NT|AES256-SHA1|AES128-SHA1|All}]
[/itercount]
[/ptype {KRB5_NT_PRINCIPAL|KRB5_NT_SRV_INST|KRB5_NT_SRV_HST}]
[/kvno <keyversionnum>]
[/answer {-|+}]
[/target]
[/rawsalt] [{-|+}dumpsalt] [{-|+}setupn] [{-|+}setpass <password>]  [/?|/h|/help]
```

#### Parameters

| Parameter | Description |
| --------- | ------------|
| /out `<filename>` | Specifies the name of the Kerberos version 5 .keytab file to generate. **Note:** This is the .keytab file you transfer to a computer that isn't running the Windows operating system, and then replace or merge with your existing .keytab file, */Etc/Krb5.keytab*. |
| /princ `<principalname>` | Specifies the principal name in the form host/computer.contoso.com@CONTOSO.COM. **Warning:** This parameter is case-sensitive. |
| /mapuser `<useraccount>` | Maps the name of the Kerberos principal, which is specified by the **princ** parameter, to the specified domain account. |
| /mapop `{add|set}` | Specifies how the mapping attribute is set.<ul><li>**Add** - Adds the value of the specified local user name. This is the default.</li><li>**Set** - Sets the value for Data Encryption Standard (DES)-only encryption for the specified local user name.</li></ul> |
| `{-|+}`desonly | DES-only encryption is set by default.<ul><li>**+** Sets an account for DES-only encryption.</li><li>**-** Releases restriction on an account for DES-only encryption. **Important:** Windows doesn't support DES by default.</li></ul> |
| /in `<filename>` | Specifies the .keytab file to read from a host computer that is not running the Windows operating system. |
| /pass `{password|*|{-|+}rndpass}` | Specifies a password for the principal user name that is specified by the **princ** parameter. Use `*` to prompt for a password. |
| /minpass | Sets the minimum length of the random password to 15 characters. |
| /maxpass | Sets the maximum length of the random password to 256 characters. |
| /crypto `{DES-CBC-CRC|DES-CBC-MD5|RC4-HMAC-NT|AES256-SHA1|AES128-SHA1|All}` | Specifies the keys that are generated in the keytab file:<ul><li>**DES-CBC-CRC** - Used for compatibility.</li><li>**DES-CBC-MD5** - Adheres more closely to the MIT implementation and is used for compatibility.</li><li>**RC4-HMAC-NT** - Employs 128-bit encryption.</li><li>**AES256-SHA1** - Employs AES256-CTS-HMAC-SHA1-96 encryption.</li><li>   **AES128-SHA1** - Employs AES128-CTS-HMAC-SHA1-96 encryption.</li><li>**All** - States that all supported cryptographic types can be used.</li></ul><p>**Note:** Because the default settings are based on older MIT versions, you should always use the `/crypto` parameter. |
| /itercount | Specifies the iteration count that is used for AES encryption. The default ignores **itercount** for non-AES encryption and sets AES encryption to 4,096. |
| /ptype `{KRB5_NT_PRINCIPAL|KRB5_NT_SRV_INST|KRB5_NT_SRV_HST}` | Specifies the principal type.<ul><li>**KRB5_NT_PRINCIPAL** - The general principal type (recommended).</li><li>**KRB5_NT_SRV_INST** - The user service instance</li><li>  **KRB5_NT_SRV_HST** - The host service instance</li></ul> |
| /kvno `<keyversionnum>` | Specifies the key version number. The default value is 1. |
| /answer `{-|+}` | Sets the background answer mode:<ul><li>**-** Answers reset password prompts automatically with **NO**.</li><li>**+** Answers reset password prompts automatically with **YES**.</li></ul> |
| /target | Sets which domain controller to use. The default is for the domain controller to be detected, based on the principal name. If the domain controller name doesn't resolve, a dialog box will prompt for a valid domain controller. |
| /rawsalt | forces ktpass to use the rawsalt algorithm when generating the key. This parameter is optional. |
| `{-|+}dumpsalt` | The output of this parameter shows the MIT salt algorithm that is being used to generate the key. |
| `{-|+}setupn` | Sets the user principal name (UPN) in addition to the service principal name (SPN). The default is to set both in the .keytab file. |
| `{-|+}setpass <password>` | Sets the user's password when supplied. If rndpass is used, a random password is generated instead. |
| /? | Displays Help for this command. |

##### Remarks

- Services running on systems that aren't running the Windows operating system can be configured with service instance accounts in AD DS. This allows any Kerberos client to authenticate to services that are not running the Windows operating system by using Windows KDCs.

- The **/princ** parameter isn't evaluated by ktpass and is used as provided. There's no check to see if the parameter matches the exact case of the **userPrincipalName** attribute value when generating the Keytab file. Case-sensitive Kerberos distributions using this Keytab file might have problems if there's no exact case match, and could even fail during pre-authentication. To check and retrieve the correct **userPrincipalName** attribute value from a LDifDE export file. For example:

    ```
    ldifde /f keytab_user.ldf /d CN=Keytab User,OU=UserAccounts,DC=contoso,DC=corp,DC=microsoft,DC=com /p base /l samaccountname,userprincipalname
    ````

#### Examples

To create a Kerberos .keytab file for a host computer that isn't running the Windows operating system, you must map the principal to the account and set the host principal password.

1. Use the active directory **User and computers** snap-in to create a user account for a service on a computer that is not running the Windows operating system. For example, create an account with the name *User1*.

2. Use the **ktpass** command to set up an identity mapping for the user account by typing:

    ```
    ktpass /princ host/User1.contoso.com@CONTOSO.COM /mapuser User1 /pass MyPas$w0rd /out machine.keytab /crypto all /ptype KRB5_NT_PRINCIPAL /mapop set
    ```

    > [!NOTE]
    > You cannot map multiple service instances to the same user account.

3. Merge the .keytab file with the */Etc/Krb5.keytab* file on a host computer that isn't running the Windows operating system.

### Additional References

- [Command-Line Syntax Key](https://github.com/MicrosoftDocs/windowsserverdocs/tree/master/WindowsServerDocs/administration/windows-commands/command-line-syntax-key.md)

---



MIT License. Copyright (c) 2020 Strontic.

