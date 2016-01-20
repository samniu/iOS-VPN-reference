#VPN相关资料
***
##VPN知识
[虚拟专用网(VPN)](https://zh.wikipedia.org/wiki/%E8%99%9B%E6%93%AC%E7%A7%81%E4%BA%BA%E7%B6%B2%E8%B7%AF)

[Proxy、SSH 和VPN 的区别](http://blog.csdn.net/map_lixiupeng/article/details/41695045)

[TUN与TAP](https://zh.wikipedia.org/wiki/TUN%E4%B8%8ETAP)

[How VPN Works](https://technet.microsoft.com/en-us/library/cc779919)

[Wiki: 隧道协议](https://zh.wikipedia.org/wiki/%E9%9A%A7%E9%81%93%E5%8D%8F%E8%AE%AE)

***运营商是怎么分析出数据通道中特定 App 的数据流量的？***

根据特定应用使用的网关IP来进行判断。曾经参与过手机QQ免流量的项目，就是把手机QQ后台所有的网关IP报到运营商处，由运营商对流量进行标记及减免。但是实施起来技术难度很大，因为用户数越多的应用IP越多，手机QQ这个统计起来非常吓人，运营商内部系统不支持非常多的IP进行标记。所以做起来技术难度很大，后期实现应该是内部对IP量进行了优化减免。 
p.s.现在似乎没法对单一用户使用某一款应用产生的流量做精确标记。
[来自知乎](https://www.zhihu.com/question/20774248/answer/16178248)

##OpenVPN
[关于OpenVPN文章的目录](http://blog.csdn.net/dog250/article/details/6990814)

[OpenVPN Documentation](https://community.openvpn.net/openvpn/wiki/TesterDocumentation)

[OpenVPN 3](https://staging.openvpn.net/openvpn3/)

[iOS-OpenVPN-Sample](https://github.com/KatekovAnton/iOS-OpenVPN-Sample)

##Shadowsocks
[shadowsocks-iOS](https://github.com/shadowsocks/shadowsocks-iOS/tree/master)

##Surge
[Surge 原理与实现](https://medium.com/@Blankwonder/surge-原理与实现-8aa3304fb3bb#.wxyp558el)

[Surge 新手使用指南](https://medium.com/@scomper/surge-%E9%85%8D%E7%BD%AE%E6%96%87%E4%BB%B6-a1533c10e80b#.vv3zvdtoa)

[Surge作者Twitter](https://twitter.com/Blankwonder)

[iOS神器 — Surge「人话版」功能介绍](http://laob.me/1888/)

[Surge, the missing tool for iOS](https://g.owind.com/surge-the-missing-tool-for-ios/)

##iOS Network Extension
[Network Extension Framework Reference](https://developer.apple.com/library/ios/documentation/NetworkExtension/Reference/Network_Extension_Framework_Reference/)

[Create an on-demand VPN connection programmatically in iOS 8](http://ramezanpour.net/post/2014/10/15/create-an-on-demand-vpn-connection-programmatically-in-ios-8/)

[Configure and manage VPN connections programmatically in iOS 8](http://ramezanpour.net/post/2014/08/03/configure-and-manage-vpn-connections-programmatically-in-ios-8/)

[WWDC: What's New in Network Extension and VPN](https://developer.apple.com/videos/play/wwdc2015-717/)

[NEVPNManager Class Reference](https://developer.apple.com/library/ios/documentation/NetworkExtension/Reference/NEVPNManagerClassRef/)

[Demo: VPNTool](https://github.com/avreolko/VPNTool)

[Demo: VPNOn](https://github.com/lexrus/VPNOn)

**Enabling Personal VPN (iOS, Mac)**

Enable personal VPN to allow your app to create and control a custom system VPN configuration using the Network Extension framework.
    

**To enable Personal VPN**

1. In the Capabilities pane, if Personal VPN isn’t enabled, click the switch in the Personal VPN section.
![4_enablepersonalvpn_2x](https://developer.apple.com/library/ios/documentation/IDEs/Conceptual/AppDistributionGuide/Art/4_enablepersonalvpn_2x.png)

2. Xcode automatically provisions your app to use personal VPN and adds the Network Extension framework to your project for you.

For information about the Network Extension framework, read [Network Extension Framework Reference](https://developer.apple.com/library/ios/documentation/NetworkExtension/Reference/Network_Extension_Framework_Reference/index.html#//apple_ref/doc/uid/TP40016234).

**iOS SDK的VPN API方案(仅支持iOS8以上)：**

功能：系统全局代理；on-demand按需配置代理；

OpenVPN:系统全局代理(任何iOS系统都支持)

shadowsocks：支持iOS8以上， iOS9不支持；



























