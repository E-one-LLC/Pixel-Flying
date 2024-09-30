首先感谢 各大佬的 技术分享   感兴趣的可以 看看
1、 @nat   [Google one vpn在pc端和移动端无限使用指南](https://linux.do/t/topic/61729)
2、友站 大佬Check [现阶段GoogleOneVpn连接问题与信息汇总](https://bbs.yummy.best/t/topic/467)
3、友站 大佬Check [大陆可以直连“Google的VPN”？GoogleOneVpn评测和想法](https://bbs.yummy.best/t/topic/81)

上述内容都是基于Google One VPN时期产出的，一些使用要求也是在Google One VPN独有的。

现在的Google VPN 没有了之前独有的使用要求，在体验上更好。

为了各位Pixel7+用户，更好的体验Googl VPN，结合大佬的[思路](https://bbs.yummy.best/t/topic/221/5)，

所以才有了以下保姆级的教程。

现在 ！

即刻开始 ！！

手把手教程！！！

[文字版步骤说明](https://linux.do/t/topic/219068)

以v2RayNG作为飞机，自备机场，飞行线路选US为例

# 1 、修改 APN接入点 代理和端口

**设置**—**网络和互联网**—**SIM 卡**—**中国移动**—**接入点名称**— **+**  修改接入点

（APN 、MCC 、MNC 、APN 类型、APN 协议、APN 漫游协议全部按原有的中国移动 GPRS 填写）

**名称**  填写 自定义

**代理** 填写 **127.0.0.1** 

**端口** 填写 **10809**  端口可以自定义

保存 

![APN 代理设置|225x500, 100%](https://cdn.jsdelivr.net/gh/E-one-LLC/Image@main/1%20APN%20%E4%BB%A3%E7%90%86%E8%AE%BE%E7%BD%AE.jpg)

# 2、修改 v2rayNG 仅代理和端口

v2rayNG设置     

左上角 **三** — **设置**

**进阶设置** 

**http代理端口** 填写 **10809** （与APN端口相同）

**模式** 选用 **仅代理**

**路由设置**  **域名策略**  选用 **IPIfNonMatch**

**预定义规则** 选用 **绕过局域网及大陆代理而后代理**

**自定义规则** **代理的网址或 IP** 填写

***.cloud.cupronickel.goog,**

***.googleapis.com,**

***.gstatic.com**

![v2rayNG 仅代理模式设置](https://cdn.jsdelivr.net/gh/E-one-LLC/Image@main/2%20v2rayNG%20%E4%BB%85%E4%BB%A3%E7%90%86%20%E6%A8%A1%E5%BC%8F%20%E8%AE%BE%E7%BD%AE.jpg)
![v2rayNG 路由设置|225x500](https://cdn.jsdelivr.net/gh/E-one-LLC/Image@main/3%20v2rayNG%20%E8%B7%AF%E7%94%B1%E8%AE%BE%E7%BD%AE.jpg)
![自定义规则|225x500](https://cdn.jsdelivr.net/gh/E-one-LLC/Image@main/3%20%E8%87%AA%E5%AE%9A%E4%B9%89%E8%A7%84%E5%88%99.png)


# 3、机场订阅链接导入  更新订阅 测试配置真连接 节点选择 这种基操 就省略了 

# 4、 打开Google VPN 准备起飞
**设置**—**网络和互联网**—**VPN**—内置 **Google VPN**

![Google VPN 打开路径|225x500](https://cdn.jsdelivr.net/gh/E-one-LLC/Image@main/4%20Google%20VPN%20%E6%89%93%E5%BC%80%E8%B7%AF%E5%BE%84.jpg)


![7ba345b45c68ce6f36a12120135011c|225x500](https://cdn.jsdelivr.net/gh/E-one-LLC/Image@main/4%20Google%20VPN%20%E4%BB%8B%E7%BB%8D.png)


![674c223a668d917bb937c4af0293095|225x500](https://cdn.jsdelivr.net/gh/E-one-LLC/Image@main/4%20Google%20VPN%20%E8%AF%B4%E6%98%8E.png)




**使用VPN**

![5 Google 连接ing|225x500](https://cdn.jsdelivr.net/gh/E-one-LLC/Image@main/5%20Google%20%E8%BF%9E%E6%8E%A5ing.jpg)



![6 Google 连接成功|225x500](https://cdn.jsdelivr.net/gh/E-one-LLC/Image@main/6%20Google%20%E8%BF%9E%E6%8E%A5%E6%88%90%E5%8A%9F.jpg)


# 5、关闭v2rayNG、恢复APN

![7 V2rayNG 停止服务|225x500](https://cdn.jsdelivr.net/gh/E-one-LLC/Image@main/7%20V2rayNG%20%E5%81%9C%E6%AD%A2%E6%9C%8D%E5%8A%A1.jpg)
![8 APN 设置选回|225x500](https://cdn.jsdelivr.net/gh/E-one-LLC/Image@main/8%20APN%20%E8%AE%BE%E7%BD%AE%E9%80%89%E5%9B%9E.jpg)


至此，只要你不主动关闭Google VPN，不开启其他VPN，手机不重启/关机，不打开飞行模式，Google VPN 就不会断开。

根据近期的使用体验，在Pixel上的Google VPN 比之前的Google One VPN好用一万倍。主要是之前Google One VPN的各种在线验证，网络波动的影响都不见了。

下面 放一下 在Wifi环境下的测试截图 

![fast 测速|225x500](https://cdn.jsdelivr.net/gh/E-one-LLC/Image@main/fast%20%E6%B5%8B%E9%80%9F.jpg)
![科技大 V4测试|225x500](https://cdn.jsdelivr.net/gh/E-one-LLC/Image@main/%E7%A7%91%E6%8A%80%E5%A4%A7%20V4%E6%B5%8B%E8%AF%95.jpg)
![科技大 V6测试|225x500](https://cdn.jsdelivr.net/gh/E-one-LLC/Image@main/%E7%A7%91%E6%8A%80%E5%A4%A7%20V6%E6%B5%8B%E8%AF%95.jpg)


按照我的使用感受，就是你的网络有多快，Google VPN的速度就有多快。
下面放一下我的 近期流量使用情况，基本上是全天候在线。
![9 近期数据使用情况|225x500](https://cdn.jsdelivr.net/gh/E-one-LLC/Image@main/9%20%E8%BF%91%E6%9C%9F%E6%95%B0%E6%8D%AE%E4%BD%BF%E7%94%A8%E6%83%85%E5%86%B5.jpg)

# 重要说明：
飞机线路的选择，一定要在[下列地区](https://support.google.com/pixelphone/answer/2819573?sjid=140733030294803112-NC#zippy=%2C%E5%8F%AF%E4%BD%BF%E7%94%A8-vpn-%E7%9A%84%E5%9B%BD%E5%AE%B6%E5%9C%B0%E5%8C%BA)中，才行。
（PS：我有个南极的线路，也开启成功了，查询IP是澳大利亚，所以只要您的线路不离谱，开启成功，是没有问题的。）

# 不重要的说明
1、第1、2、3步先后顺序对第4步无影响。

2、第5步先后顺序无影响。

3、对于第5步飞机关闭和恢复APN，经使用体验，如果不关闭和恢复APN的话，对某信使用会有影响，比如说有些小程序会拒绝访问，图片加载失败。

4、端口可自定义，但是最好不要和常用端口冲突。


# 使用拓展

一、 在WIFI环境下，您可以[在Pixel 设备上连接到 Google VPN](https://support.google.com/pixelphone/answer/2819573?sjid=140733030294803112-NC#zippy=)后， 配合[Every Proxy](https://play.google.com/store/apps/details?id=com.gorillasoftware.everyproxy&pcampaignid=web_share)将Google VPN网络共享到局域网（在[Edge](https://www.microsoft.com/zh-cn/edge?form=MA13FJ)、[Chrome](https://www.google.cn/intl/zh-CN/chrome/)上配合[SwitchyOmega](chrome-extension://padekgcemlokbadohgkifijomclgjgif/options.html#!/about)使用）。

二、[Root的手机使用相关模块达到Pixel 使用Google VPN的效果](https://linux.do/t/topic/220413)。
（先给自己埋个坑，等11月份推出保姆级教程，使用Pixel 2 XL 测试一下）

三、如果不选择使用手机修改APN，也可以在Wifi环境下使用代理，实现前置代理，或者您用更高阶的路由实现前置代理。
