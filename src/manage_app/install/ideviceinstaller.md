# ideviceinstaller

## help语法

```bash
➜  ~ ideviceinstaller --help
Usage: ideviceinstaller OPTIONS

Manage apps on iOS devices.

OPTIONS:
  -u, --udid UDID    Target specific device by UDID.
  -n, --network        Connect to network device.
  -l, --list-apps    List apps, possible options:
       -o list_user    - list user apps only (this is the default)
       -o list_system    - list system apps only
       -o list_all    - list all types of apps
       -o xml        - print full output as xml plist
  -i, --install ARCHIVE    Install app from package file specified by ARCHIVE.
                           ARCHIVE can also be a .ipcc file for carrier bundles.
  -U, --uninstall APPID    Uninstall app specified by APPID.
  -g, --upgrade ARCHIVE    Upgrade app from package file specified by ARCHIVE.
  -L, --list-archives    List archived applications, possible options:
       -o xml        - print full output as xml plist
  -a, --archive APPID    Archive app specified by APPID, possible options:
       -o uninstall    - uninstall the package after making an archive
       -o app_only    - archive application data only
       -o docs_only    - archive documents (user data) only
       -o copy=PATH    - copy the app archive to directory PATH when done
       -o remove    - only valid when copy=PATH is used: remove after copy
  -r, --restore APPID    Restore archived app specified by APPID
  -R, --remove-archive APPID  Remove app archive specified by APPID
  -o, --options        Pass additional options to the specified command.
  -w, --notify-wait        Wait for app installed/uninstalled notification
                            to before reporting success of operation
  -h, --help        prints usage information
  -d, --debug        enable communication debugging
  -v, --version        print version information

Homepage:    <https://libimobiledevice.org>
Bug Reports: <https://github.com/libimobiledevice/ideviceinstaller/issues>
```
