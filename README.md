# Autoruns

Autoruns aims to parse the auto startup location in Windows registry keys on offline system.It's consisting of 13 parsers. Each parser represents a category, as illustrated in below table.

| Parser        | Discribtion                               | Registry hive  |
| ------------- |:-----------------------------------------:| --------------:|
|AppinitDLLs| Lists all DLLs that will be arbitrary loaded into each user mode process on the system.    | SYSTEM & SOFTWARE |
|BootExecute| Lists Windows native-mode executables that are started by the Session Manager (Smss.exe) during system boot.      | SYSTEM |
|   Codecs  | Lists executable code that can be loaded by media playback applications.     | SOFTWARE & NTUSER |
| Explorer  | Lists common autostart entries that hook directly into Windows Explorer.      |   SYSTEM |
|ImageHijacks| Image hijacks means running a different program from the one you specify and expect to be running. The Image Hijacks parser lists four types of these redirections: <br />exefile: Changes to the association of the .exe or .cmd file types with an executable command.<br />htmlfile: Changes to the association of the .htm or .html file types with an executable command.<br />Command: Processor\Autorun A command line that is executed whenever a new Cmd.exe instance is launched.<br />Image File Execution Options: One purpose for IFEO subkeys that has been documented is the ability to specify an alternate program to start whenever a particular application is launched. | SOFTWARE & NTUSER |
| BootExecute   | Lists Windows native-mode executables that are started by the Session Manager (Smss.exe) during system boot.      |   SYSTEM |
| BootExecute   | Lists Windows native-mode executables that are started by the Session Manager (Smss.exe) during system boot.      |   SYSTEM |
| BootExecute   | Lists Windows native-mode executables that are started by the Session Manager (Smss.exe) during system boot.      |   SYSTEM |
| BootExecute   | Lists Windows native-mode executables that are started by the Session Manager (Smss.exe) during system boot.      |   SYSTEM |
| BootExecute   | Lists Windows native-mode executables that are started by the Session Manager (Smss.exe) during system boot.      |   SYSTEM |
| BootExecute   | Lists Windows native-mode executables that are started by the Session Manager (Smss.exe) during system boot.      |   SYSTEM |
| BootExecute   | Lists Windows native-mode executables that are started by the Session Manager (Smss.exe) during system boot.      |   SYSTEM |
| BootExecute   | Lists Windows native-mode executables that are started by the Session Manager (Smss.exe) during system boot.      |   SYSTEM |

