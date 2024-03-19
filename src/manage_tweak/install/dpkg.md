# dpkg

* dpkg
  * 安装过程分很多步骤
    * TODO：把多个步骤整理过来

* 概述
  * 安装deb `-i` == `-install`
    ```bash
    dpkg -i xxx.deb
    ```
  * 卸载deb `-r` == `-remove`
    ```bash
    dpkg -r xxx.deb
    ```
  * 查看deb信息 `-s` == `-see`
    ```bash
    dpkg -s xxx.deb
    ```

## 用dpkg安装deb

### 举例

* Reveal2Loader
  ```bash
  dpkg -i Reveal2Loader_1.0-6_iphoneos-arm.deb
  ```
* theos
  ```bash
  dpkg -i /tmp/_theos_install.deb
  ```
* iOSGods
  ```bash
  dpkg -i "/var/mobile/Documents/com.iosg.mobs_5.25+iOSGods.com_iphoneos-arm.deb"
  ```
* 其他
  ```bash
  dpkg -i "/var/root/当当关注查件17.8-9.deb"
  ```

## dpkg版本信息

* iPhone8-150
  ```bash
  iPhone8-150:~ root# which dpkg
  /usr/bin/dpkg
  iPhone8-150:~ root# dpkg --version
  Debian 'dpkg' package management program version 1.21.9 (iphoneos-arm).
  This is free software; see the GNU General Public License version 2 or
  later for copying conditions. There is NO warranty.
  ```
* Crifan-iPhone6
  ```bash
  ➜  ~ ssh root@192.168.0.54
  Crifan-iPhone6:~ root# which dpkg
  /usr/bin/dpkg
  Crifan-iPhone6:~ root# dpkg --version
  Debian 'dpkg' package management program version 1.19.7 (iphoneos-arm).
  This is free software; see the GNU General Public License version 2 or
  later for copying conditions. There is NO warranty.
  ```


## dkpg相关命令工具

* dpkg
* dpkg-deb
* dpkg-divert
* dpkg-genbuildinfo
* dpkg-query
* dpkg-split
* dpkg-trigger

->

* XinaA15越狱后的iPhone11中

```bash
iPhone11-151:~ root# ls -lh /private/preboot/3B92D6F7C3FE6444A715B312E418498574E442DAB2F6D9E18B58B762F71D1455B7E2E1C2DD3912B1B4E6D10C6B9150C8/procursus/usr/bin/
...
-rwxrwxrwx 1 root wheel 116K Feb  2 21:55 dpkg*
-rwxrwxrwx 1 root wheel  72K Feb  2 21:55 dpkg-deb*
-rwxrwxrwx 1 root wheel 172K Jan 18 15:08 dpkg-divert*
-rwxr-xr-x 1 root wheel  21K Jan 18 15:08 dpkg-maintscript-helper*
-rwxrwxrwx 1 root wheel  89K Feb  2 21:55 dpkg-query*
-rwxr-xr-x 1 root wheel 4.1K Jan 18 15:08 dpkg-realpath*
-rwxrwxrwx 1 root wheel 169K Jan 18 15:08 dpkg-split*
-rwxrwxrwx 1 root wheel 112K Jan 18 15:08 dpkg-statoverride*
-rwxrwxrwx 1 root wheel 115K Jan 18 15:08 dpkg-trigger*
```

* 使用Termux部署Python3的Android系统中

```bash
$ ls -l usr/bin/
...
-rwx------    1 u0_a260  u0_a260     265696 Jul  1 13:56 dpkg
-rwx------    1 u0_a260  u0_a260     134416 Jul  1 13:56 dpkg-deb
-rwx------    1 u0_a260  u0_a260     134320 Jul  1 13:56 dpkg-divert
-rwx------    1 u0_a260  u0_a260      16822 Jul  1 13:56 dpkg-genbuildinfo
-rwx------    1 u0_a260  u0_a260     134312 Jul  1 13:56 dpkg-query
-rwx------    1 u0_a260  u0_a260     134128 Jul  1 13:56 dpkg-split
-rwx------    1 u0_a260  u0_a260      68560 Jul  1 13:56 dpkg-trigger
```

