本页面最近一次更新时间：2020.03.13
### passwall官方telegram频道（源码更新内容、x86_64/x86官方编译固件分发）：       
[主频道](https://t.me/passwall)            
### passwall固件分发分频道汇总：             
[分频道](./sub.md)               
### 主要由Lienol<猛禽>维护的源码Lienol/openwrt（有分支）可供你自行编译属于你的设备的定制化固件:             
[源码](./code.md)                   
### 符合F22起降标准的“机场”：    
暂无推荐         
[推荐标准：有IPLC韩国视频节点、支持月付][本站只推荐一个相比最好的。当节点波动且不及时优化时，会更换推荐]             
机场主可以联系：[群管理](https://t.me/wefuxkgfw),参与竞标。                

------------------------------------------------------------------------------------
### 临时贴士：            
* 如果改过LAN口的IP后上不了网，请重启软路由。     
### 小贴士：       
[使用官方编译固件做视频教程，讲解固件使用相关任意方面的UP，可以把视频链接发到频道关联的群中，当猛禽Lienol看过觉得可以时，将作为本页面永久推荐教程]   
* 不保留配置升级：[图文](./upgrade.md)                 
* 请务必保持启用passwall的高级设置里的守护进程！           
* 长期接受类gfwlist分流规则推荐，请在issues区推荐给Lienol<猛禽>：                        
[https://github.com/Lienol/openwrt/issues](https://github.com/Lienol/openwrt/issues)                                
* 不允许访客使用代理、自由指定不同客户端使用不同线路、盒子看Netflix：               
[https://youtu.be/qkga9DN5H08](https://youtu.be/qkga9DN5H08)             
* 如何DDNS外网无需加端口远程访问 dynuDNS解析 URL转发 治愈强迫症：  
[https://youtu.be/c4HSZzTM7G0](https://youtu.be/c4HSZzTM7G0)         
* 单线or双线，最简单的iptv内网融合教程，需要懂一点基础：      
[https://github.com/luckyyyyy/blog/issues/44](https://github.com/luckyyyyy/blog/issues/44)            
* 手动单独更新passwall按钮不要一直使用，当出问题后还是需要完整不保留配置刷入最新完整固件的，否则依赖包不会更新，无法修复bug和获得优化体验          
* 如果出现YouTube等一些网站的页面上的特定内容错误显示，比如广告区域加载失败，只有框框没有图片，大概率是你的系统（不是固件！）的负责域名快速解析的HOSTS文件在作妖，解决办法是删除HOSTS文件里的所有规则（# 号注释掉的内容可以不管，其他的都删掉）               
* 单臂路由模式下，如果无法访问国内网站，尝试在网络防火墙自定义规则添加这条规则（请注意要求eth0为LAN口）：            
iptables -t nat -I POSTROUTING -o eth0 -j MASQUERADE           
或者这条规则（有桥接存在的情况下）：       
iptables -t nat -I POSTROUTING -o  br-lan  -j MASQUERADE            
* 始终无法连接到软路由网络、始终无网络：[可能解决办法](./winproxy.md)               
* 科学上网测速注意：[注意事项](./speed.md)                  

