## Linux File System Hierarchy

[![Picture](./assets/filesystem.png)](./assets/filesystem.png)


- **/ :** Root directory, All other directories and files are under this directory.

- **/boot :** contains everything required for boot.

- **/bin :** store basic commands and binaries like `ls` `cp` `cat` `rm` for regular users.

- **/sbin :** store `root` (system admin) user commands like `fdisk` `fsck` `ifconfig`. these commands can be run without root user.

- **/lib (libraries) :** store shared programs required by programs in `/bin` and `/sbin`.

- **/usr :** contains executables, libraries, man etc files.
  - **/usr/bin :** contains user-level executable binaries that are available to all users like `node` `python3` `vim` but they are not essential for system startup.
  - **/usr/sbin :** contains user-level executable binaries but they require `superuser` privileges like `apachectl` `sshd` `ntpd`.
  - **/usr/lib :** store shared programs for `/usr/bin` and `/usr/sbin` binaries like `/usr/lib/python3.9`.
  - **/usr/local :** used to install software manually by the system administrator (Not managed by the system's package manager).
  - **/usr/share :** `data files` `documentation` `icons` that are shared by multiple applications.
    - **/usr/share/icons :** application icons.
    - **/usr/share/man :** manual pages.
    - **/usr/share/doc :** documentation.
  - **/usr/include :** header files for C and C++ programming `stdio.h`.
  - **/usr/src :** source code for applications and kernel headers. used for `customizing` the Linux kernel.

- **/etc (configuration files) :** contains system and installed applications configuration files like `/etc/nginx/nginx.conf` `/etc/apache2/apache2.conf` `/etc/networks` `/etc/group`.

- **/root :** home directory for the `root` (superuser or system admin) account.

- **/home :** contains personal directories for users like the user `ck` would have `/home/ck`. can be used for storing `download` `image` `sound` files etc.

- **/dev (devices) :** contains devices files like `hardware` `printer` `usb`
  - **/dev/sda :** hard disk partitions like `sda1` `sda2`.
  - **/dev/cdroom :** `cdroom` partition.
  - **/dev/psaux :** `mouse` `keyboard` devices files.
  - **/dev/lp0 :** `printer` `scanner` devices files.
  - **/dev/usb :** `usb` devices files.

- **/media and /mnt (Mount Points) :** temporary mount points for removable media like `usb drives` or `external hard drives`.

- **/opt (Optional Software) :** common location for installing additional software packages that are not part of the default installation.

- **/proc (Process Information) :** contains information about system processes and kernel like `/proc/cpuinfo` `/proc/meminfo`.
 
- **/var :** contains variable data files like `logs` `cache` `web application files` `lock` `temp files`.
  - **/var/log :** store system and application log files.
  - **/var/tmp :** store temporary files created by various processes.
  - **/var/cache :** store cache files used by applications to improve performance.
  - **/var/lib :** store state information for various services and applications.
  - **/var/www :** store web application related files.

- **/tmp :** contains temporary files created by applications or the system. This directory is cleared out at boot or at shutdown.

