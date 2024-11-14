# ActiveX Controls Fix
An effort to fix ActiveX errors on Windows 10 + 11

This fix contains 147 ActiveX Controls (.OCX files) that are missing or unregistered on Windows 10 and 11. These files are installed to 

C:\Windows\SysWOW64

These .OCX files will not be removed or unregistered if you uninstall this fix, many of them are present in some form already and only need to be registered. This installer accounts for that and adjusts which files it installs accordingly.

If you do not have the Visual Basic 4.0, 5.0 and 6.0 runtimes installed, some of these registrations may fail. If you encounter registration errors, it is best to download and install Retro Windows Game Dependencies (RWGD) from one of the mirrors below. It contains all three of the required Visual Basic runtimes. After doing this, you can run this installer again and you should not get any, or very few errors (less than 5 is normal, you can press ignore and the installer will continue). If you get more than 5 registration errors with RWGD installed, please let me know on the LGU Discord.

RWGD Mirror 1 (Google Drive)

https://drive.google.com/file/d/1Z0qE-5v7XuOCCwi9boyAw3qiRW3Foc_A

RWGD Mirror 2 (NAS)

https://os5.mycloud.com/action/share/462d5f2b-5c89-4f8b-b277-2dfcc23e4a58

LGU Discord

https://discord.com/invite/wF3zJPDVQg





Info for nerds


1. This only installs on 64 bit systems, since 32 bit Windows hasn't existed since the early days of 10 and also doesn't have a SysWOW64 folder
2. If any of the .OCX files are already present, it doesn't touch or overwrite them - it only digitally signs, sets the system file flag, and registers them (regsvr32 registration)
3. It doesn't remove or uninstall any of the .OCX files if you uninstall it - this would be dangerous because I believe a small amount of these are required for Windows' operation even still today
4. The way my installer creation program (Caphyon's Advanced Installer 16.3) works, I had to have one file in a program directory, so there's a dummy .txt file installed to 'C:\Program Files\ActiveX Controls Fix' - coincidentally this is the only thing that actually gets removed when you "uninstall" this fix
5. I'm fairly certain that the Visual Basic 4.0, 5.0, 6.0 runtimes are not the only dependencies this requires, but I've had a few other people test it after installing RWGD with minimal (less than 5, zero on some systems) errors out of 145 files - these registration errors are because there's a companion .DLL for the .OCX missing in 'C:\Windows\SysWOW64'
6. I'm aware that people know how to fix .OCX errors already, I just don't think that anyone has provided a comprehensive fix like this for pretty much all of them
7. If you really want to, you can track down all the components of RWGD and install them rather than installing it - here's the contents of RWGD

   • DirectInput Mapper (Microsoft)

   • DirectX 8.0 Redistributable (Microsoft)

   • DirectX 8.1 Redistributable (Microsoft)

   • DirectX 9 June 2010 Redistributable (Microsoft)

   • _inmm.dll v2.3.0.8 - cryo.jp/_inmm

   • .NET 1.1 Redistributable (Microsoft)

   • .NET 4.0 SlimDX Redistributable (Microsoft)

   • OpenAL v1.1 - openal.org

   • RAD Video Tools - radgametools.com/bnkdown.htm

   • Visual Basic 4.0 Redistributable (Microsoft)

   • Visual Basic 5.0 Redistributable (Microsoft)

   • Visual Basic 6.0 Runtime Plus by rizalmart - sourceforge.net/u/rizalmart

   • Visual C++ Redistributables [2005 thru 2022 - x86/x64] (Microsoft)

   • Windows Media Source Filter (DirectShow Codec) by mrpenguinb - community.pcgamingwiki.com/profile/3946-mrpenguinb

   • WinG (Microsoft)

   • WinG32 (Microsoft)
