### passwall官方telegram频道（源码更新内容、x86_64/x86官方编译固件分发）：       
[https://t.me/passwall](https://t.me/passwall)              

------------------------------------------------------------------------------------         
### 符合F22起降标准的“机场”：         
招标考察中       

------------------------------------------------------------------------------------
### 小贴士：       
[使用官方编译固件做视频教程，讲解固件使用相关任意方面的UP，可以把视频链接发到频道关联的群中，当猛禽Lienol看过觉得可以时，将作为本页面永久推荐教程]     
* 请务必保持启用passwall的高级设置里的守护进程！      
* 长期接受类gfwlist分流规则推荐，请在issues区推荐给Lienol（有分流方面的强烈建议也可以）：[https://github.com/Lienol/openwrt/issues](https://github.com/Lienol/openwrt/issues)             
* 不允许访客使用代理、自由指定不同客户端使用不同线路、盒子看Netflix：[https://youtu.be/qkga9DN5H08](https://youtu.be/qkga9DN5H08)        
* 如何DDNS外网无需加端口远程访问 dynuDNS解析 URL转发 治愈强迫症：[https://youtu.be/c4HSZzTM7G0](https://youtu.be/c4HSZzTM7G0)        
* 单线or双线，最简单的iptv内网融合教程，需要懂一点基础：[https://github.com/luckyyyyy/blog/issues/44](https://github.com/luckyyyyy/blog/issues/44)        
* 手动单独更新passwall按钮不要一直使用，当出问题后还是需要完整不保留配置刷入最新完整固件的，否则依赖包不会更新，无法修复bug和获得优化体验          
* 如果出现YouTube等一些网站的页面上的特定内容错误显示，比如广告区域加载失败，只有框框没有图片，大概率是你的系统（不是固件！）的负责域名快速解析的HOSTS文件在作妖，解决办法是删除HOSTS文件里的所有规则（# 号注释掉的内容可以不管，其他的都删掉）               
* 单臂路由模式下，如果无法访问国内网站，尝试在网络防火墙自定义规则添加这条规则（请注意要求eth0为LAN口）：            
iptables -t nat -I POSTROUTING -o eth0 -j MASQUERADE           
或者这条规则（有桥接存在的情况下）：       
iptables -t nat -I POSTROUTING -o  br-lan  -j MASQUERADE            
