# MonkeyDev

* MonkeyDev（调试并安装ipa）
  * 但是会出现问题
    * 【未解决】iOS逆向AppleStore：为何MonkeyDev调试安装ipa后运行会出现各种出错
      * iOS的app，即使是 砸壳版本
        * dpkg安装ipa：（都可以）正常使用，不会出错
        * Xcode+MonkeyDev调试安装：打开后各种错误，且无法彻底解决
          * 对于Apple Store：
            * app group path问题
            * Charles抓包证书出错问题
            * （从iCloud）同步Apple账户失败
          * 对于之前的抖音
            * NSString空字符串崩溃问题
            * 等等
      * ->最后已确认是重签名期间导致entitlement权限丢失，从而导致后续运行期间出现各种问题
