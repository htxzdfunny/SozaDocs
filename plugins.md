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
| MC服务器状态查询 | mc | 某猫 | 提供MineCraft JE/BE版服务器状态查询。| [跳转](./) |
| 网页截图模块 | webscreen | 某猫 | 快速获取指定网页图片。 | [跳转](./) |
| Planet ACGN Journey 剧情游戏模块 | paj | 某猫&Misaka12456 | [暂未开放]无说明。 | 无 |


### 小泽核心(sozacore)  
这里面有很多奇奇怪怪的东西..小泽也不知道为什么会有这些奇奇怪怪东西..  
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

`/arc help` -调出此帮助菜单  
`/arc bind <arcid>` -绑定您的arcid(指九位数字好友ID 下同)  
`/arc unbind` -解绑  
`/arc userinfo [at|arcid]` -查询账号详情  
`/arc info [at|arcid]` -查询最近打谱  
/`arc best <曲名> [Future(默认)|Present|Past]` -查询单曲最佳（目前暂不可用）  
`/arc b30` -查询best30（目前暂不可用）  

### Cytoid铲车模块(ctd)
> 有被踢的觉悟，才有资格写谱   
> 这个八月的贵阳永远不会怒拆额！！  

`/ctd help` -调出此帮助铲车  
`/ctd bind <uid>` -绑定您的我会怒拆额  
`/ctd unbind` -退群！  
`/ctd image [at|uid]` -获取鸡E句NBA（暂不可用）  
`/ctd userinfo [at|uid]` -查询阿格王朔详情（暂不可用）  
`/ctd [info] [at|uid]` -查询最近紫薯布丁  

> 注：帮助铲车=帮助菜单；我会怒拆额=阿格王朔=账号；退群=解绑；鸡E句NBA=头像；最近紫薯布丁=最近打歌  

### Osu戳泡泡模块(osu)
> 祝您滑条必断  

`/osu help` -调出帮助菜单  
`/osu setid <id>` -绑定您的osu账号  
`/osu pf:[mode] [id/at]` -查某人在某模式的个人信息  
`/osu pr:[mode] [id/at]` -查某人在某模式杀的歌  
`/osu mode: <0-3>` -切换你的主模式  
`/osu 更新个签 <内容>` -更换您pf上的个性签名  
`/osu 更新背景` -更新您pf的背景  

> 您知道吗：切换主模式的参数既可以是0-3，也可以是以下几种：  
> [![yfYDgO.png](https://s3.ax1x.com/2021/02/19/yfYDgO.png)](https://imgchr.com/i/yfYDgO)


> 本页面尚未完成，当前展示仅为预览版，不代表最终品质。