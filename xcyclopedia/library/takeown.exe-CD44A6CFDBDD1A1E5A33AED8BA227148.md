﻿
# takeown.exe 
* File Path: `C:\WINDOWS\SysWOW64\takeown.exe`
* Description: Takes ownership of a file
* Comments: 

## Hashes
Type | Hash
-- | --
MD5 | `CD44A6CFDBDD1A1E5A33AED8BA227148`
SHA1 | `6D124C3F37F2A9A09163E95A2AC64F4292F4E3B7`
SHA256 | `A6780DC8D060DC4C629EFBE5FFE4B545E5476A80017D86B7A79BC5CCC1DE47AD`
SHA384 | `5066A6045FEE719045FE2D6B839B3830BDA520A19D457F779B7E3237110F448062AFA93545400DD569FB652CCD8BBA8B`
SHA415 | `BA8E8DB9401EA129CE39D80BC1B117B74CF30563A1D456F178AFA76CF1C3EB43A2EA476C9091D731AB331BE611910BBC06D22D335A9E8DF00B713A4953DE4AFC`
SSDEEP | `1536:83WkghEw/BWqjjKCnhTTbdEme6i939WhpWfkZa817:RM8nh3hQ6i9N8pOkZa8`

## Runtime Data
### Usage (stdout):
```Batchfile

TAKEOWN [/S system [/U username [/P [password]]]]
        /F filename [/A] [/R [/D prompt]]

Description:
    This tool allows an administrator to recover access to a file that
    was denied by re-assigning file ownership.

Parameter List: 
    /S           system          Specifies the remote system to
                                 connect to.

    /U           [domain\]user   Specifies the user context under
                                 which the command should execute.

    /P           [password]      Specifies the password for the
                                 given user context.
                                 Prompts for input if omitted.

    /F           filename        Specifies the filename or directory
                                 name pattern. Wildcard "*" can be used
                                 to specify the pattern. Allows
                                 sharename\filename.

    /A                           Gives ownership to the administrators
                                 group instead of the current user.

    /R                           Recurse: instructs tool to operate on
                                 files in specified directory and all 
                                 subdirectories.

    /D           prompt          Default answer used when the current user
                                 does not have the "list folder" permission
                                 on a directory.  This occurs while operating
                                 recursively (/R) on sub-directories. Valid 
                                 values "Y" to take ownership or "N" to skip.

    /SKIPSL                      Do not follow symbolic links.
                                 Only applicable with /R.

    /?                           Displays this help message.

    NOTE: 1) If /A is not specified, file ownership will be given to the
             current logged on user.

          2) Mixed patterns using "?" and "*" are not supported.

          3) /D is used to suppress the confirmation prompt.

Examples: 
    TAKEOWN /?
    TAKEOWN /F lostfile
    TAKEOWN /F \\system\share\lostfile /A
    TAKEOWN /F directory /R /D N
    TAKEOWN /F directory /R /A
    TAKEOWN /F *
    TAKEOWN /F C:\Windows\System32\acme.exe
    TAKEOWN /F %windir%\*.txt
    TAKEOWN /S system /F MyShare\Acme*.doc
    TAKEOWN /S system /U user /F MyShare\MyBinary.dll
    TAKEOWN /S system /U domain\user /P password /F share\filename
    TAKEOWN /S system /U user /P password /F Doc\Report.doc /A
    TAKEOWN /S system /U user /P password /F Myshare\* 
    TAKEOWN /S system /U user /P password /F Home\Logon /R
    TAKEOWN /S system /U user /P password /F Myshare\directory /R /A

```

### Usage (stderr):
```Batchfile
ERROR: Invalid argument/option - '-help'.
Type "TAKEOWN /?" for usage.

```

### Child Processes:


## Signature

* Status: Signature verified.
* Serial: 330000023241FB59996DCC4DFF000000000232
* Thumbprint: FF82BC38E1DA5E596DF374C53E3617F7EDA36B06
* Issuer: CN=Microsoft Windows Production PCA 2011, O=Microsoft Corporation, L=Redmond, S=Washington, C=US
* Subject: CN=Microsoft Windows, O=Microsoft Corporation, L=Redmond, S=Washington, C=US

## File Metadata

* Original Filename: takeown.exe
* Product Name: Microsoft Windows Operating System
* Company Name: Microsoft Corporation
* File Version: 10.0.18362.1 (WinBuild.160101.0800)
* Product Version: 10.0.18362.1
* Language: English (United States)
* Legal Copyright:  Microsoft Corporation. All rights reserved.

