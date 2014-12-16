Relevance Cheat Sheet
=====================

OS expressions
--------------

### Mac

    Q: name of operating system
    A: Mac OS X
    T: 37

    Q: name of operating system contains "Mac"
    A: True
    T: 42

    Q: name of operating system contains "os"
    A: False
    T: 44

    Q: name of operating system contains "OS"
    A: True
    T: 45

    Q: name of operating system contains "ac"
    A: True
    T: 43

    Q: version of operating system
    A: 10.9.5
    T: 57

    Q: (name of it, version of it) of operating system
    A: Mac OS X, 10.9.5
    T: 68

    Q: architecture of operating system
    A: x86_64
    T: 35

    Q: windows of operating system
    A: False
    T: 38

    Q: unix of operating system
    A: False
    T: 45

    Q: mac of operating system
    A: True
    T: 36

    Q: (exists matches (regex "^Sun|^Linux Red|^AIX") of it) of name of operating system
    A: True
    T: 6858

### Windows

    Q: name of operating system
    A: Win2008R2
    T: 0.039 ms

    Q: version of operating system
    A: 6.1.7601
    T: 0.048 ms

    (sometimes service pack is tricky on windows, Windows XP x64 only goes to service pack 2 but not 1  or something like that if I remember correctly)
    Q: service pack major version of operating system A: 1
    T: 0.041 ms

Reg apps (registered applications)
----------------------------------

### Windows

    Q: names of regapps
    A: 7zFM.exe
    A: AcroRd32.exe
    A: BESConsole.exe
    A: dexplore.exe
    A: firefox.exe
    A: iediagcmd.exe
    A: iediagcmd.exe
    A: iexplore.exe
    A: javaws.exe
    A: notepad++.exe
    A: vsta.exe
    A: WinMergeU.exe
    A: WinMergeU.exe
    A: WinRAR.exe
    T: 14.435 ms

    Q: (names of it, versions of it) of regapps
    A: 7zFM.exe, 9.20.0.0
    A: AcroRd32.exe, 11.0.9.29
    A: BESConsole.exe, 9.1.909.0
    A: dexplore.exe, 8.0.50727.1826
    A: firefox.exe, 33.0.2.5413
    A: iediagcmd.exe, 11.0.9600.16428
    A: iediagcmd.exe, 11.0.9600.16428
    A: iexplore.exe, 11.0.9600.17344
    A: javaws.exe, 10.67.2.1
    A: notepad++.exe, 6.5.1.0
    A: vsta.exe, 9.0.30729.1
    A: WinMergeU.exe, 2.12.4.0
    A: WinMergeU.exe, 2.12.4.0
    A: WinRAR.exe, 5.1.0.0
    T: 16.024 ms

#### Does this file exist?

    Q: name of operating system
    A: Win2008R2
    T: 0.039 ms

    Q: exists file "C:\windows\system32\drivers\etc\hosts"
    A: True
    T: 0.147 ms

    Q: exists file "C:\Windows\system32\drivers\etc\nothosts"
    A: False
    T: 0.182 ms

    Q: lines of file "C:\Windows\system32\drivers\etc\hosts"
    A: # Copyright (c) 1993-2009 Microsoft Corp.
    A: #
    A: # This is a sample HOSTS file used by Microsoft TCP/IP for Windows.
    A: #
    A: # This file contains the mappings of IP addresses to host names. Each
    A: # entry should be kept on an individual line. The IP address should
    A: # be placed in the first column followed by the corresponding host name.
    A: # The IP address and the host name should be separated by at least one
    A: # space.
    A: #
    A: # Additionally, comments (such as these) may be inserted on individual
    A: # lines or following the machine name denoted by a '#' symbol.
    A: #
    A: # For example:
    A: #
    A: #      102.54.94.97     rhino.acme.com          # source server
    A: #       38.25.63.10     x.acme.com              # x client host
    A:
    A: # localhost name resolution is handled within DNS itself.
    A: #%09127.0.0.1       localhost
    A: #%09::1             localhost
    A:
    A: 9.39.144.15%09ecengvc01.bigfix.com
    A:
    A:
    A: # Comment out this by Terry
    A: # 67.134.15.13%09daemonspawn.bigfix.com
    A: # END
    T: 0.611 ms

    Q: line 3 of file "C:\Windows\system32\drivers\etc\hosts"
    A: # This is a sample HOSTS file used by Microsoft TCP/IP for Windows.
    T: 0.263 ms

### On a mac

    Q: exists file "/private/etc/hosts"
    A: True
    T: 92

    Q: exists file "/private/etc/nothosts"
    A: False
    T: 140

    Q: number of lines of file "/private/etc/hosts"
    A: 10
    T: 175

Is the user logged in?
----------------------

    Q: names of logged on users
    A: dex
    T: 419

    Q: name of current user
    A: dex
    T: 205

### Terminal Server

    Q: names of logged on users
    A: shuo_li
    A: bilgehan_sahin
    A: yang_meng
    A: bao_nhan
    A: yunfei_bai
    A: sylvia_yangbin
    A: chuxin_zhao

    Q: current user
    E: Singular expression refers to nonexistent object.

What’s a path of one of the special system directories?
-------------------------------------------------------

### Mac

    Q: name of system folder
    A: System
    T: 117

    Q: pathname of system folder
    A: /System
    T: 44

    Q: pathname of users folder
    A: /Users

    Q: pathname of applications folder
    A: /Applications

### Windows

    Q: pathname of windows folder
    A: C:\Windows
    T: 0.185 ms

    Q: pathname of system folder
    A: C:\Windows\system32
    T: 0.189 ms

    Q: pathname of system x32 folder
    A: C:\Windows\system32
    T: 0.179 ms

    Q: pathname of system x64 folder
    A: C:\Windows\system32
    T: 0.179 ms

    Q: pathname of system wow64 folder
    A: C:\Windows\SysWOW64
    T: 0.192 ms

    Q: pathname of program files folder
    A: C:\Program Files (x86)
    T: 0.150 ms

    Q: pathname of program files x32 folder
    A: C:\Program Files (x86)
    T: 0.152 ms

    Q: pathname of program files x64 folder
    A: C:\Program Files
    T: 0.168 ms

    Q: pathname of data folder of client
    A: C:\Users\dexter_liu\Downloads\FixletDebugger-9.2.0.363\__BESData
    T: 0.258 ms

Does this registry key exist
----------------------------

    Q: exists key "HKLM\Software\Bigfix\EnterpriseClient\Settings" of registry
    A: True
    T: 0.087 ms

Remember on wow64 systems it could be slightly different... x64 registry

    Q: values of key "HKLM\Software\Bigfix\EnterpriseClient\Settings\Client\_BESClient_LastShutdown_Reason" of registry

A: Service manager shutdown request A: Thu, 23 Oct 2014 16:36:44 -0700
T: 0.166 ms

    Q: (names of it, it) of values of key "HKLM\Software\Bigfix\EnterpriseClient\Settings\Client\_BESClient_LastShutdown_Reason" of registry
    A: value, Service manager shutdown request
    A: effective date, ( Thu, 23 Oct 2014 16:36:44 -0700 )
    T: 0.185 ms

    Q: names of keys of key "HKLM\Software\Bigfix\EnterpriseClient\Settings\Client" of registry
    A: _BESClient_LastShutdown_Reason
    A: _BESClient_Resource_StartupNormalSpeed
    A: _BESClient_UploadManager_BufferDirectory
    A: _BESDataServer_APIAuthenticationTimeoutMinutes
    A: _BESDataServer_AuthenticationTimeoutMinutes
    A: _BESGather_Comm_UseDownloadService
    A: _BESGather_Download_CacheLimitMB
    ...
    A: __Relay_Control_Server2
    T: 1.008 ms

Is the registry key this value (version \#, is this version 3 or higher?)
-------------------------------------------------------------------------

    Q: (value "Version" of it) of key "HKLM\Software\Bigfix\EnterpriseClient" of registry
    A: 42.0.85.0
    T: 0.120 ms

    Q: (value "Version" of it > "42") of key "HKLM\Software\Bigfix\EnterpriseClient" of registry
    A: True
    T: 0.102 ms

    Q: (value "Version" of it > "43") of key "HKLM\Software\Bigfix\EnterpriseClient" of registry
    A: False
    T: 0.092 ms

Is this application installed?
------------------------------

    Q: values "DisplayName" of keys of key "HKLM\Software\Microsoft\Windows\CurrentVersion\Uninstall" of registry
    A: Adobe Flash Player 11 ActiveX
    A: Google Chrome
    A: IBM Installation Manager
    A: IBM Rational Team Concert Client
    A: IBM Endpoint Manager Server
    ...
    A: Perforce Visual Components
    A: Microsoft Visual C++ 2008 Redistributable - x86 9.0.21022
    T: 142.635 ms

    Q: exists key whose (value "DisplayName" of it as string as lowercase contains "google chrome") of key "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall" of native registry
    A: True
    T: 0.301 ms

    Q: exists key whose (value "DisplayName" of it as string as lowercase contains "google chromes") of key "HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Uninstall" of native registry
    A: False
    T: 1.734 ms

How much disk space is free?
----------------------------

### Mac

    Q: free space of volume "Macintosh HD"
    A: 402534928384
    T: 154

### Windows

    Q: (free spaces of it, names of it) of drives
    A: 53851201536, C:
    T: 438.227 ms

Does this text exist in a text file?
-----------------------------------
Reading a config file to see what a value is, or see if it’s the expected value

    Q: lines of file "C:\Windows\system32\drivers\etc\hosts"
    A: # Copyright (c) 1993-2009 Microsoft Corp.
    A: #
    A: # This is a sample HOSTS file used by Microsoft TCP/IP for Windows.
    A: #
    A: # This file contains the mappings of IP addresses to host names. Each
    A: # entry should be kept on an individual line. The IP address should
    A: # be placed in the first column followed by the corresponding host name.
    A: # The IP address and the host name should be separated by at least one
    A: # space.
    A: #
    A: # Additionally, comments (such as these) may be inserted on individual
    A: # lines or following the machine name denoted by a '#' symbol.
    A: #
    A: # For example:
    A: #
    A: #      102.54.94.97     rhino.acme.com          # source server
    A: #       38.25.63.10     x.acme.com              # x client host
    A:
    A: # localhost name resolution is handled within DNS itself.
    A: #%09127.0.0.1       localhost
    A: #%09::1             localhost
    A:
    A: 9.39.144.15%09ecengvc01.bigfix.com
    A:
    A:
    A: # Comment out this by Terry
    A: # 67.134.15.13%09daemonspawn.bigfix.com
    A: # END
    T: 0.611 ms

    Q: content of file "C:\WIndows\system32\drivers\etc\hosts" contains "9.39.144.15"
    A: True

    Q: content of file "C:\WIndows\system32\drivers\etc\hosts" contains "9.39.144.16"
    A: False

Is an application installed on a mac (mac specific inspector)
-------------------------------------------------------------

    ### Same inspectors work on mac
    Q: (names of it, versions of it) of regapps
    A: Dota 2.app, 1.0
    A: GitHub.app, Medium Hefson
    A: Adium.app, 1.5.10
    A: Adobe Reader.app, 11.0.9
    A: App Store.app, 1.3
    A: AT&T Global Network Client Uninstaller.app, 1.0
    A: AT&T Global Network Client.app, 1.5.0.3024
    A: Automator.app, 2.4
    A: Balsamiq Mockups.app, 2.2.22
    A: Calculator.app, 10.8
    T: 300655

References to time
------------------

### DATE

    Q: now
    A: Sun, 16 Nov 2014 18:49:28 -0800
    T: 1007

    Q: now + 1*day
    A: Mon, 17 Nov 2014 18:50:02 -0800
    T: 56

    Q: now + 2*day
    A: Tue, 18 Nov 2014 18:50:06 -0800
    T: 49

    Q: current date
    A: Sun, 16 Nov 2014
    T: 43

    Q: current date + 5 * day
    A: Fri, 21 Nov 2014
    T: 40

    Q: "16 Nov 2014" as date < (current date + 5*day)
    A: True
    T: 64

    Q: "16 Nov 2014" as date < (current date + 1*day)
    A: True
    T: 64

    Q: "16 Nov 2014" as date < (current date)
    A: False
    T: 50

### TIME

    Q: now
    A: Sun, 16 Nov 2014 18:57:27 -0800
    T: 3281

    Q: now - 5*hour
    A: Sun, 16 Nov 2014 13:57:30 -0800
    T: 47

    Q: modification time of file "/Users/Dex/Relevance Cheat Sheet"
    A: Sun, 16 Nov 2014 18:54:37 -0800
    T: 115

    Q: modification time of file "/Users/Dex/Relevance Cheat Sheet" > now - 5*hour
    A: True
    T: 51

    Q: modification time of file "/Users/Dex/Relevance Cheat Sheet" > now
    A: False
    T: 46

Network objects, mac address, IP address
----------------------------------------

    Q: addresses whose (it as string != "0.0.0.0") of ip interfaces of network as string  =

    A: 127.0.0.1
    A: 192.168.1.102
    A: 9.80.109.49
    T: 305

    Q: (mac addresses of it, addresses of it) of ip interfaces of network as string
    A: 3c-15-c2-b7-c7-1a, 192.168.1.102
    T: 209

    Q: (name of it, mac addresses of it, addresses of it) of ip interfaces of network as string
    A: en0, 3c-15-c2-b7-c7-1a, 192.168.1.102
    T: 302

Primitives
----------
Casting a string, version, dealing with dates (reading in a date from a file and turning into a bf date, or dealing with a bf date) – what’s a bf date, needs to get it into a specific format, or turn it into, what month this says it is – dates way more complex than they need to be, mod date for a file (need just day/month/year)

    Casting date from string:
    Q: current date
    A: Sun, 16 Nov 2014
    T: 0.037 ms
    I: singular date

    Q: current date + 1*day
    A: Mon, 17 Nov 2014
    T: 0.049 ms
    I: singular date

    Q: current date as string
    A: Sun, 16 Nov 2014
    T: 0.056 ms
    I: singular string

    Q: (current date as string) + 1*day
    E: The operator "plus" is not defined.

    Q: "Sun, 16 Nov 2014"
    A: Sun, 16 Nov 2014
    T: 0.039 ms
    I: singular string

    Q: "Sun, 16 Nov 2014" + 1*day
    E: The operator "plus" is not defined.

    Q: "Sun, 16 Nov 2014" as date + 1*day
    A: Mon, 17 Nov 2014
    T: 0.116 ms
    I: singular date

There's a weird thing with version comparisons too but I forgot what it
was

### File modified within the last 30 days:

    Q: (names of it, modification times of it) of files of folder "C:\Users\Bigfix\Downloads"
    A: agnc.msi, ( Tue, 17 Jun 2014 17:41:19 -0800 )
    A: attachment_14784920_UnmanagedAssetsWithFilters.besrpt, ( Thu, 24 Oct 2013 16:16:25 -0800 )
    A: BESAdmin (1).exe, ( Mon, 30 Jun 2014 22:13:34 -0800 )
    A: BESAdmin.exe, ( Mon, 30 Jun 2014 21:41:50 -0800 )
    A: BESClientSetupMSI.exe, ( Mon, 07 Jul 2014 10:32:55 -0800 )
    A: BESConsole.exe, ( Mon, 30 Jun 2014 21:50:47 -0800 )
    A: BESGather (1).exe, ( Mon, 30 Jun 2014 21:52:27 -0800 )
    T: 9.980 ms
    I: plural ( string, time )

    Q: (names of it, modification times of it) of files whose (now - modification time of it < 30*day) of folder "C:\Users\Bigfix\Downloads"
    A: FixletDebugger-9.2.0.363.zip, ( Fri, 14 Nov 2014 10:43:37 -0800 )
    A: QNA9.2.0.375.zip, ( Fri, 07 Nov 2014 01:09:53 -0800 )
    T: 9.614 ms
    I: plural ( string, time )

### Getting day month year from modification time of a file:

    Q: modification time of file "C:\Users\Bigfix\Downloads\QNA9.2.0.375.zip"
    A: Fri, 07 Nov 2014 01:09:53 -0800
    T: 0.348 ms
    I: singular time

    Q: modification time of file "C:\Users\Bigfix\Downloads\QNA9.2.0.375.zip" as date
    E: The operator "date" is not defined.

    Q: (year of it as string & "/" & month of it as two digits & "/" & day_of_month of it as two digits) of date (local time zone) of modification time of file "C:\Users\Bigfix\Downloads\QNA9.2.0.375.zip"
    A: 2014/11/07
    T: 0.391 ms
    I: singular string

Are services running, do they exist
-----------------------------------

I think service stuff is only for windows

    Q: exists service "BESClient"
    A: True
    T: 0.053 ms
    I: singular boolean

    Q: state of service "BESClient"
    A: Running
    T: 0.078 ms
    I: singular string

    Q: service "BESClient"
    A: "BESClient" "BES Client" "Running"
    T: 0.084 ms
    I: singular service

    Q: all services
    A: "1394ohci" "1394 OHCI Compliant Host Controller" "Stopped"
    A: "ACPI" "Microsoft ACPI Driver" "Running"
    A: "AcpiPmi" "ACPI Power Meter Driver" "Stopped"
    A: "adp94xx" "adp94xx" "Stopped"
    A: "adpahci" "adpahci" "Stopped"
    ...
    A: "WwanSvc" "WWAN AutoConfig" "Stopped"
    T: 86.738 ms
    I: plural service

Is this process running?
------------------------

### Windows

    Q: (names of it, pids of it, ids of it) of processes
    A: System Idle Process, 0, 0
    A: System, 4, 4
    A: taskhost.exe, 3504, 3504
    A: rdpclip.exe, 3792, 3792
    A: dwm.exe, 2512, 2512
    A: explorer.exe, 4076, 4076
    A: vmtoolsd.exe, 3240, 3240
    A: BESClientUI.exe, 2928, 2928
    A: ssmsee.exe, 3016, 3016
    A: sublime_text.exe, 6020, 6020
    A: chrome.exe, 4456, 4456
    A: chrome.exe, 5912, 5912
    A: chrome.exe, 1724, 1724
    A: FixletDebugger.exe, 4012, 4012
    A: regedit.exe, 192, 192
    A: BESConsole.exe, 5244, 5244
    T: 3.347 ms
    I: plural ( string, integer, integer )

### Mac

    Q: (names of it, ids of it, pids of it, process id of it) of processes
    A: mdworker, 604, 604, 604
    A: mdworker, 603, 603, 603
    A: mdworker, 602, 602, 602
    A: mdworker, 601, 601, 601
    A: Google Chrome He, 598, 598, 598
    A: QnA, 591, 591, 591
    A: bash, 588, 588, 588
    ...
    A: com.apple.InputM, 286, 286, 286

Event log – show me the events with this ID in the application log
------------------------------------------------------------------

    Q: (time generated of it, (if exists description of it then description of it else "NA")) of records whose (event id of it mod 65536 = 1 AND now - time generated of it < 5*day) of application event log  =

    A: ( Wed, 12 Nov 2014 06:44:01 -0800 ), The Windows Security Center Service has started.
    T: 1631.353 ms
    I: plural ( time, string )

    Q: number of records whose (event id of it mod 65536 = 7036 AND now - time generated of it < 1*day) of system event log

    A: 30075
    T: 8365.912 ms
    I: singular integer

// this one is tricky and is due to a weird windows glitch

To get this working I think you'll need to find an example to work with
where the error is available in the event log.

When you have an example, you'll need to mod the event ID by 2\^15 or
2\^30 most likely, but you'll have to experiment to see what ends up
matching the IDs in your event viewer.

Windows ends up throwing away the highbits of stuff
<http://msdn.microsoft.com/en-us/library/aa363651.aspx>

which means we end up with event ids different than event viewer
typically:
<https://www.ibm.com/developerworks/community/forums/html/topic?id=77777777-0000-0000-0000-000014748770>
=

> So basically the event viewer in Windows throws away the "high bits"
> of the event, but the event ID inspector doesn't do this. According to
> the Microsoft technical documentation, the bits of the "EventID" looks
> like this: <http://msdn2.microsoft.com/en-us/library/aa363651.aspx> .
> As far as we can tell, you aren't technically supposed to throw away
> the high bits of the event id so we are having a hard time calling
> this a full bug, but it seems to me that we should allow you to get
> the Event Viewer's concept of the ID that doesn't include the
> high-bits.

    Q: exists records whose (event id of it = 7036) of event log "system"  =

    A: False
    T: 7684.630 ms
    I: singular boolean

    Q: number of records whose (now - time generated of it < 3*day) of system event log
    A: 1090
    T: 10088.286 ms
    I: singular integer

WMI – serial number of computer, or serial number for a computer for a mac
--------------------------------------------------------------------------

### Mac

    Q: string "IOPlatformSerialNumber" of dictionary of service plane of iokit registry
    A: C02MF1BKFD59
    T: 236

### Windows

    Q: if (exists wmi) then (string values of selects "SerialNumber from Win32_BIOS" of wmi) else ("N/A")
    A: VMware-56 4d 2f f4 23 f3 d2 3f-7a b7 1c 5a 10 d0 1d f5
    T: 8.366 ms
    I: plural string

This one should work for UNIX (haven't tested though) if (exists dmi AND
exists serial\_number of system\_information of dmi) then
(serial\_number of system\_information of dmi)

Version Comparisons
-------------------

The minimum length is all that's compared. So as the left side has less
elements then that is all thats compared.

    Q: version "9" = version "9.1.2.3"
    A: true

    Q: version "9.1" = version "9.1.2.3"
    A: true

1 or 2 examples of plurals, an example of it, 2 example of a tuple
------------------------------------------------------------------

### Tuples

    Q: subnet addresses of adapters of network
    A: 9.39.115.0
    A: 127.0.0.0
    T: 3395

    Q:  ((substrings separated by "." of (it as string)) of subnet addresses of adapters of network)
    A: 9
    A: 39
    A: 115
    A: 0
    A: 127
    A: 0
    A: 0
    A: 0
    T: 220

    Q: ((concatenation ", " of substrings separated by "." of (it as string)) of subnet addresses of adapters of network)
    A: 9, 39, 115, 0
    A: 127, 0, 0, 0
    T: 206

    Q:  tuple string items of ((concatenation ", " of substrings separated by "." of (it as string)) of subnet addresses of adapters of network)
    A: 9
    A: 39
    A: 115
    A: 0
    A: 127
    A: 0
    A: 0
    A: 0
    T: 245

    Q:  tuple string items 1 of ((concatenation ", " of substrings separated by "." of (it as string)) of subnet addresses of adapters of network)
    A: 39
    A: 0
    T: 1540

    Q:  tuple string items 0 of ((concatenation ", " of substrings separated by "." of (it as string)) of subnet addresses of adapters of network)
    A: 9
    A: 127
    T: 204

Another example I want to translate CSV + tuples:
<https://www.ibm.com/developerworks/community/forums/html/topic?id=77777777-0000-0000-0000-000014747527>

In line relevance for action script
-----------------------------------

A common use case is to "When an action runs, I want to tag something
with the runtime of the action."

     regset "[HKEY_LOCAL_MACHINE\SOFTWARE\BigFix\Actions]" "Runtime"="{now}"

Of course, this is a pretty good reference to put in here to that talks
about escape brackets and stuff in actionscript:
<http://www-01.ibm.com/support/docview.wss?uid=swg21506259>

You can also use relevance substitution to run specific executables on
your file system with the special bigfix file directory inspectors.

    run "{pathname of windows folder}\notepad.exe"
    run "{pathname of parent folder of regapp "myapp.exe"}\myapp.exe"
    run "{value "PathToEXE" of key "HKLM\Software\MyApp" of registry}"
    run "{pathname of regapp "otherapp.exe"}"

Actually, this whole entire guide was pretty good references here:
<https://www.ibm.com/developerworks/community/wikis/home?lang=en#!/wiki/Tivoli%20Endpoint%20Manager/page/BigFix%20Actions>

Comments
--------

Comments are double-slashes: //

    // Action to stop the Messenger service so that users do not receive
    // spam-like message pop-ups

    dos net stop "Messenger"

Actually all of the restrictions and gotchas and caveats are covered
fairly well here:
<https://www.ibm.com/developerworks/community/wikis/home?lang=en#!/wiki/Tivoli%20Endpoint%20Manager/page/BigFix%20Actions>

Concatenation (relevance)
-------------------------

    q: (name of it & ": " & it as string) of values of key "HKEY_LOCAL_MACHINE\SOFTWARE\Bigfix\EnterpriseClient" of registry
    A: EnterpriseClientFolder: C:\Program Files\BigFix Enterprise\BES Client\
    A: Version: 42.0.85.0
    T: 0.391 ms

Other good relevance reference materials
----------------------------------------

<https://www.ibm.com/developerworks/community/wikis/home?lang=en#!/wiki/Tivoli%20Endpoint%20Manager/page/Relevance%20Tips>
<https://www.ibm.com/developerworks/community/wikis/home?lang=en#!/wiki/Tivoli%20Endpoint%20Manager/page/Property%20%26%20Relevance%20Examples>
