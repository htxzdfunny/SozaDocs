# 模块列表

## 模块简要介绍
- 小泽的功能其实由多个模块实现，各个模块互相依赖且互不干扰。
- 考虑到小泽的消息解析方式与开发者的技术力，分模块也许是目前最佳的解决方案。  

## 模块列表  

| 名称 | 模块Id | 开发者 | 说明 | 帮助链接 |
|  ----  | ----  | ---- | ---- | ---- |
| 小泽核心 | sozacore | 某猫 | [默认开启，状态不可操作]顾名思义，是小泽的底层核心。负责各个模块的通讯与脑机互联。| [跳转](./plugins?id=小泽核心sozacore) |
| 数据库模块 | db | 某猫 | [默认开启，状态不可操作]顾名思义，是小泽的数据库操作模块。| 无 |
| Arcaea模块 | arc | 某猫 | 提供Arcaea相关信息查询。| [跳转](./plugins?id=arcaea玩蛇模块arc) |
| Cytoid模块 | ctd | 某猫 | 提供Cytoid相关信息查询。| [跳转](./plugins?id=cytoid铲车模块ctd) |
| Osu!模块 | osu | 某猫&Shatnine\(629\) | 提供Osu相关信息查询。 | [跳转](./plugins?id=osu戳泡泡模块osu) |
| MC服务器状态查询 | mc | 某猫 | 提供MineCraft JE/BE版服务器状态查询。| [跳转](./plugins?id=minecraft服务器状态查询mc) |
| 网页截图模块 | webscreen | 某猫 | 快速获取指定网页图片。 | [跳转](./) |
| Planet ACGN Journey 剧情游戏模块 | paj | 某猫&Misaka12456 | [暂未开放]无说明。 | 无 |
| Fujao-Time报时模块 | paj | 某猫&冰糖酱(BillZhou233) | 符语报时模块。 | [跳转](./plugins?id=fujao-time贵阳报时模块fjt) |


### 小泽核心(sozacore)  
这里面有很多奇奇怪怪的东西..小泽也不知道为什么会有这些奇奇怪怪的东西..  
#### 主帮助菜单(/z help)
`/z help [data]` -调出主帮助菜单或请求的帮助菜单  
`/z rhythm` -调出音游相关功能  
`/z paolu` -调出跑团相关功能  
`/z tools` -一些工具类指令  
`/z <stat|status>` -查询小泽的运行状态  
`/z repeat <内容>` -给姐姐（某猫）说小泽的坏话（雾  
#### 音游类菜单(/z rhythm)
`/arc help` -Arcaea模块菜单  
`/ctd help` -Cytoid模块菜单   
`/osu help` -Osu!模块菜单  
#### 工具类菜单(/z tools)  

`/z set pm <on|off>` -设置是否接收全体广播  
`/z pluginlist` -模块列表  
`/z set plugin <appId> <this/groupId> <true/false>` -设置某模块在某群的启用状态  
`/mc help` -MC服务器状态查询  

### Arcaea玩蛇模块(arc)
> 真人面对面收割 美女角色在线掉分 发狂玩蛇新天地  

**使用须知**

> Arcaea是由lowiro limited开发的一款 3D 立体下落式音乐游戏。  
本模块与 Arcaea，lowiro limited 无从属关系。  
您应知悉，使用本模块的相关指令将违反 Arcaea 使用条款中的 3.2-4 和 3.2-6，以及 Arcaea 二次创作管理条例。  
因使用本模块的相关指令而造成的损失，小泽及小泽开发者不予承担任何责任。  

`/arc help` -调出此帮助菜单  
`/arc bind <arcid>` -绑定您的arcid(指九位数字好友ID 下同)  
`/arc unbind` -解绑  
`/arc userinfo [at|arcid]` -查询账号详情  
`/arc info [at|arcid]` -查询最近打谱  
`/arc best <曲名> [Future(默认)|Present|Past]` -查询单曲最佳（目前暂不可用）  
`/arc b30` -查询best30（目前暂不可用）  

### Cytoid铲车模块(ctd)
> 有被踢的觉悟，才有资格写谱   
这个八月的贵阳永远不会怒拆额！！  

`/ctd help` -调出此帮助铲车  
`/ctd bind <uid>` -绑定您的我会怒拆额  
`/ctd unbind` -退群！  
`/ctd image [at|uid]` -获取鸡E句NBA（暂不可用）  
`/ctd userinfo [at|uid]` -查询阿格王朔详情（暂不可用）  
`/ctd [info] [at|uid]` -查询最近紫薯布丁  

**注：帮助铲车=帮助菜单；我会怒拆额=阿格王朔=账号；退群=解绑；鸡E句NBA=头像；最近紫薯布丁=最近打歌**   

### Osu戳泡泡模块(osu)
> 祝您滑条必断（逃  

**使用须知**  

> Osu!是由peppy (Dean Herbert) 开发的一款Windows平台上的同人节奏游戏。  
本模块使用了官方提供的osu-api。  
因使用本模块的相关指令而造成的损失，小泽及开发者 不予承担任何责任。  

*Supported By Shatnine & 沙茶酱 & Sayobot & 某猫*  

`/osu help` -调出帮助菜单  
`/osu setid <id>` -绑定您的osu账号  
`/osu pf[:mode] [id/at]` -查某人在某模式的个人信息  
`/osu pr[:mode] [id/at]` -查某人在某模式最近一次杀的歌  
`/osu bp[1-100]` -查你的bestPlay记录(100以内)  
`/osu mode <0-3>` -切换你的主模式  
`/osu 更新个签 <内容>` -更换您pf资料卡上的个性签名  
`/osu 更新背景` -更新您pf资料卡的背景  

> 使用实例:  
> `/osu setid xiaofang2333` -绑定一个叫做xiaofang2333的账号  
> `/osu pf htxzdfunny` -查询htxzdfunny在默认模式下的个人资料卡  
> `/osu pr:1 sayobot` -查询sayobot在taiko模式下的最近打歌  
> `/osu mode 骂娘` -将您的默认查分模式切换成模式3(即mania)

> 您知道吗：切换主模式的参数既可以是0-3，也可以是以下几种：  
> ![yfYDgO.png](https://s3.ax1x.com/2021/02/19/yfYDgO.png)


### MineCraft服务器状态查询(mc)  

`/mc [help]` -模块帮助  
`/mc bind <je/be> <ip> <port>`  -绑定本群的JE/BE服务器  
`/mc <je/be> [ip] [port]` -查询一个je/be服务器状态  

> 范例:
> `/mc bind be mcbe.qmqaq.top 25565` -将一个be服务器绑定到本群  
> `/mc je` -查本群绑定的je服务器在线状态  
> `/mc je dabaiyun.net 30412` -查这个je服务器的状态  

> 您知道吗：JE(java)版服务器默认端口为25565  

### 网页截图模块(webscreen)  
Not open.

### Fujao-Time贵阳报时模块(fjt)  
> 您知道吗：本模块为Cytoid定制版，且由于该企划为2020年策划，句子库中部分句子可能已经过于陈旧。  

> 句子库地址[点这](https://github.com/fujao-time/fujaoese-hitokoto)

`/fjt [help]` -调出帮助菜单  
`/fjt gl add [groupId]` -添加群订阅  
`/fjt gl del [groupId]` -删除群订阅  
`/fjt <ver|version>` -获取句子库版本  
`/fjt get` -获取一条随机fujao  
`/fjt chanche` -投稿句子  
**注意:使用gladd与gldel时，指定groupId需要权限 ≥ Bot协作者**
> 范例:  
> `/fjt gl add` -在本群订阅fujao-time报时  
> `/fjt gl del 1145141919` -删除群1145141919的订阅  


> 本页面尚未完成，当前展示仅为预览版，不代表最终品质。