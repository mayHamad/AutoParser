# Autoruns

Autoruns aims to parse the auto startup location in Windows registry keys on offline system. It's consisting of 13 parsers. Each parser represents a category, as illustrated in below table.

| **Parser**        | **Discribtion**                               | **Registry hive**  |
| :-------------: |:-----------------------------------------| :--------------:|
|AppinitDLLs| Lists all DLLs that will be arbitrary loaded into each user mode process on the system.    | SYSTEM<br />SOFTWARE |
|BootExecute| Lists Windows native-mode executables that are started by the Session Manager (Smss.exe) during system boot.      | SYSTEM |
|Codecs| Lists executable code that can be loaded by media playback applications.     | SOFTWARE<br />NTUSER |
|Explorer| Lists common autostart entries that hook directly into Windows Explorer.      | SOFTWARE<br />NTUSER  |
|ImageHijacks| Image hijacks means running a different program from the one you specify and expect to be running. The Image Hijacks parser lists four types of these redirections: <br />**exefile:** Changes to the association of the .exe or .cmd file types with an executable command.<br />htmlfile: Changes to the association of the .htm or .html file types with an executable command.<br />**Command:** Processor\Autorun A command line that is executed whenever a new Cmd.exe instance is launched.<br />**Image File Execution Options (IFEO):** One purpose for IFEO subkeys that has been documented is the ability to specify an alternate program to start whenever a particular application is launched. | SOFTWARE<br />NTUSER  |
|InternetExplorerAddons| Internet Explorer is designed for extensibility, with interfaces specifically exposed to enable Explorer bars such as the Favorites and History bars, toolbars, and custom menu items and toolbar buttons.<br />InternetExplorerAddons parser liste all addons and xtensions that load whenever an Internet Explorer is launched. |   SOFTWARE<br />NTUSER |
|KnownDLLs| During startup, the Session Manager maps the DLLs listed in KnownDlls key into memory as named section objects. When a new process is loaded and needs to map these DLLs, it uses the existing sections rather than searching the file system for another version of the DLL.      | SYSTEM |
|Logon| Lists all scripts and binary files that will be execute when Windows starts up and a user logs on | SYSTEM<br />SOFTWARE<br />NTUSER |
|LSAsecurityProviders| Lists all DLLs that are loaded by Lsass.exe or Winlogon.exe and run as Local System. |   SYSTEM |
|OfficeAddins| Lists add-ins and plug-ins registered to hook into documented interfaces for Access, Excel, Outlook, PowerPoint, and Word.      | SOFTWARE<br />NTUSER |
|PrintMonitorDLLs| Lists all DLLs that are loaded into the Spooler service. | SYSTEM<br />SOFTWARE |
|Winogon| Lists entries that hook into Winlogon.exe, which manages the Windows interactive-logon user interface | SYSTEM<br />SOFTWARE<br />NTUSER |
|Winsock| Lists registered Winsock protocols and Winsock service providers. Malware often installs itself as a Winsock service provider | SYSTEM |

