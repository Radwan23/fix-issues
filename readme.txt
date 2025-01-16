Wampserver 3.3.7 64 bit x64
Apache 2.4.62.1 - PHP 7.4.33/8.0.30/8.1.31/8.2.26/8.3.14/8.4.0 - MySQL 9.1.0 - MariaDB 11.5.2
Also includes PhpMyAdmin 5.2.1 - Adminer 4.8.4 - PhpSysInfo 3.4.4.

--- Installation of Wampserver ---
Wampserver requires a disk or formatted NTFS partition. Does not support FAT32 or exFAT
BEFORE proceeding with the installation of Wampserver, you must ensure that certain elements are installed on your system, otherwise Wampserver will absolutely not run, and in addition, the installation will be faulty and you need to remove Wampserver BEFORE installing the elements that were missing.
Make sure you are "up to date" in the redistributable packages VC9, VC10, VC11, VC13, VC14 and VC17 (2015-2022)
See --- Visual C++ Packages below.
--- Do not install Wampserver OVER an existing version, follow the advice:
Install a new version of Wampserver: http://forum.wampserver.com/read.php?2,123606
If you install Wampserver over an existing version, not only it will not work, but you risk losing your existing databases.

--- Install Wampserver in a folder at the root of a disk, for example C:\wamp or D:\wamp. Take an installation path that does not include spaces or diacritics; Therefore, no installation in c:\Program Files\ or C:\Program Files (x86\

--- Install Wampserver "as an administrator" i.e Right-Click on installer file then Run as an administrator.

We must BEFORE installing, disable or close some applications:
- Close Skype or force not to use port 80
Item No. 04 of the Wampserver TROUBLESHOOTING TIPS http://forum.wampserver.com/read.php?2,134915
- Disable IIS
Item No. 08 of the WampserverTROUBLESHOOTING TIPS http://forum.wampserver.com/read.php?2,134915

- Visual C++ Packages
- Verify that all VC ++ packages are installed and with the latest versions.
To do this, use the tool:
https://wampserver.aviatechno.net/files/tools/check_vcredist.exe]Checks VC++ packages installed
Do not use a previously loaded tool. Make a new download to make sure you are using the correct version.
To download missing packages, do not rely on Microsoft links, they are not reliable, download packages on https://wampserver.aviatechno.net/]http://wampserver.aviatechno.net in section Visual C++ Redistribuable Packages
Do not forget that if you have a 64 bit Windows, you must install both 32 and 64 bit versions of each package.
You must install each package "as an administrator", so right-click the exe file and then run as Administrator.

If these prerequisites are not in place, Press the Cancel button to cancel the installation, then apply the prerequisites and restart the installation.

------ After Installation ------
--- PhpMyAdmin
When starting phpMyAdmin, you will be asked for a user name and password.
After installing Wampserver 3, the default username is "root" (without quotes) and there is no password, which means that you must leave the form Password box empty.
There will be a warning:
You are connected as 'root' with no password, which corresponds to the default MySQL privileged account. Your MySQL server is running with this default, is open to intrusion, and you really should fix this security hole by setting a password for user 'root'.
This is not a problem as long as access to Phpmyadmin remain locally.
However, some web applications or CMS asking that the MySQL user has a password. In which case, you will create a user with password via the PhpMyAdmin Accounts Users tab.

--- Using the menus and submenus of Wampmanager
Do not use the keyboard to navigate through the menus and submenus of Wampmanager icon.

--- For questions regarding Wampserver 3
Please use the specific English forum http://forum.wampserver.com/list.php?2
(Or French forum http://forum.wampserver.com/list.php?1 )
Do not use an existing discussion, but create your own thread: New Topic (French : Nouvelle discussion) after having read  http://forum.wampserver.com/read.php?2,129067 READ BEFORE YOU ASK A QUESTION in this forum.

Nota : It is possible to do silent install by command line 'as an administrator':
wampserver3.3.0_x86.exe /DIR="C:\wamp" /VERYSILENT /SUPPRESSMSGBOXES
or
wampserver3.3.5_x64.exe /DIR="C:\wamp" /VERYSILENT /SUPPRESSMSGBOXES
You may replace install dir.