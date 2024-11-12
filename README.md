# ActiveX-Controls-Fix
An effort to fix ActiveX errors on Windows 10 + 11

This fix contains 145 ActiveX Controls (.OCX files) that are missing or unregistered on Windows 10 and 11. These files are installed to C:\Windows\SysWOW64

These .OCX files will not be removed or unregistered if you uninstall this fix, many of them are present in some form already and only need to be registered. This installer accounts for that and adjusts which files it installs accordingly.

If you do not have the Visual Basic 4.0, 5.0 and 6.0 runtimes installed, some of these registrations may fail. If you encounter registration errors, it is best to download and install Retro Windows Game Dependencies (RWGD) from one of the mirrors below. It contains all three of the required Visual Basic runtimes. After doing this, you can run this installer again and you should not get any, or very few errors (less than 5 is normal, you can press ignore and the installer will continue). If you get more than 5 registration errors with RWGD installed, please let me know on the LGU Discord.

RWGD Mirror 1 (Google Drive)
https://drive.google.com/file/d/1Z0qE-5v7XuOCCwi9boyAw3qiRW3Foc_A

RWGD Mirror 2 (NAS)
https://os5.mycloud.com/action/share/462d5f2b-5c89-4f8b-b277-2dfcc23e4a58

LGU Discord
https://discord.com/invite/wF3zJPDVQg
