# 命令列表  

## 观前提示

!> **注意:在阅读本文之前，请您务必先阅读[观前提示](./qa)。**  

**但是我猜你不会看 所以我复制一遍（**

必填参数用`<>`包裹。  
选填参数用`[]`包裹。  
而`|`代表“或”。

所有的参数之间都以空格分隔，参数是可选的。  

指令其它包含的特殊符号，如 ^（脱字符）、$、/（斜杠）、%（百分号）等，为自动填充的格式或符号，与包裹的符号与竖线一样，并不需要出现在指令中。

实例：  
`/ctd info htxzfunny -q 3` 这是正确的√。  
`/z <stat>` 这是错误的×，包裹的符号不需要打出来。  
`/ctd set mode image|text` 这是错误的×，`image|text`意思是你应该从`image`或者`text`中选择一个填入。

> 手机端用户可以点左下角展开目录

## 基础功能(base)  

- `/z` 存活测试
- `/z help` 调出帮助菜单
- `/z <stat|status>` 运行状态
- `/z about` 关于小泽Bot
- `/report <内容>` 问题反馈
- `/dismiss @小泽` 令小泽主动退群（权限要求≥群管理员)

## 音游信息查询(rhythm)

### Arcaea信息查询(arc)  

本模块基于[Project Andreal](https://www.showdoc.com.cn/andrea/)搭建

指令列表请点击[这里](https://www.showdoc.com.cn/andrea/7380927562006836)查看

### Cytoid信息查询(ctd)  

特别鸣谢:Tigerhix Neo BillZhou233(冰糖酱) Sunset'  

- `/ctd help` 调出模块菜单
- `/ctd ping` 检查伺服器连通性
- `/ctd bind <uid>` 绑定你的游戏账号
- `/ctd unbind` 无需参数，一键解绑账号
- `/ctd pf [uid|@]` 查询自己或他人的个人信息，如 rt/等级 等  
&nbsp;&nbsp;&nbsp;&nbsp;实例：`/ctd pf tigerhix` 查询 "tigerhix" 的个人信息  
- `/ctd info [uid|@] -q <N>` 查询自己或他人的最近第N条游玩记录(仅ranked mode，N≤10 且 ∈Z)*（开发中 可能不完善）*  
&nbsp;&nbsp;&nbsp;&nbsp;实例：`/ctd info miyou379 -q 2` 查询 "miyou379" 倒数第二条游玩记录  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`/ctd info -q 5` 查询绑定账号的倒数第五条游玩记录  
- `/ctd` --查询自己的最近游玩记录
- `/ctd set mode <image|text>` --切换图片/文字模式(仅对RecentPlay生效)*（开发中 可能不完善）*  
&nbsp;&nbsp;&nbsp;&nbsp;实例：`/ctd set mode image` 将您的默认输出模式改为图片模式  
&nbsp;&nbsp;&nbsp;&nbsp;![切换图片模式](https://cdn.u1.huluxia.com/g4/M01/25/68/rBAAdmG3QcCANSfLAAA0ypDCusc326.png)  

### Project Sekai 信息查询(pjsk)  

本模块基于[Project Andreal](https://www.showdoc.com.cn/andrea/)搭建

指令列表请点击[这里](https://www.showdoc.com.cn/andrea/8032032802988301)查看  

<!-- 
## MaiMai

模块魔改自：[Diving-Fish/mai-bot](https://github.com/Diving-Fish/mai-bot)  

- `今日舞萌` -看看今天的舞萌运势  
- `XXXmaimaiXXX什么` -随机一首歌  
- `随个[绿黄红紫白]<难度>` -随机一首指定条件的乐曲  
- `查歌<乐曲标题的一部分>` -查询符合条件的乐曲  
- `[绿黄红紫白]id<歌曲编号>` -查询乐曲信息或谱面信息  
- `<歌曲别名>是什么歌` -查询乐曲别名对应的乐曲  
- `定数查歌 <定数>` -查询定数对应的乐曲  
- `定数查歌 <定数下限> <定数上限>`  
- `分数线 <难度+歌曲id> <分数线>` 详情请输入“分数线 帮助”查看  
- `我是二次元 [用户名]` -查b40

!> 注意：使用b40前，请先在[查分器](https://www.diving-fish.com/maimaidx/prober/)导入数据并绑定您的QQ
-->

## 群管系统(gm)  

!> 本模块处于测试阶段，如有问题请及时反馈。  

- `/gm` 群管菜单
- `/gm set welcome [this|groupId]` 开始设置指定群入群欢迎  
  
入群欢迎可用变量如下:  

- `[qq]`被操作者QQ(纯文本)
- `[trigqq]`操作者QQ(纯文本)
- `[atqq]`艾特被操作者QQ
- `[attrigqq]`艾特操作者QQ
- `[time]`操作时间
- `[head]`被操作者头像
- `[trighead]`操作者头像  

<!-- TODO- `/gm query welcome [this|groupId]` 查询指定群入群欢迎
-->
## 图片生成(image)  

### 基本玩法

- `致电<名称> <@某人>` 致电某人
- `高情商 <内容> 低情商 <内容>` 高低情商
- `捏<我|QQ|@某人>` 捏捏某人的头像  
- `橙黑 <橙色内容> <黑色内容>` 生成一张橙黑图(DDDD

除此以外，还有一些进阶玩法：  

### 调用 PlantUML 绘图  

[PlantUML中文用户手册](https://plantuml.com/zh/guide)  

使用例子如下：  

```
@startuml
Alice -> Bob: test
@enduml
```

以下是一个实例:  

![实例](https://p1.meituan.net/csc/7cfe10d9f3771cbdb6b5e7c4286e707e12538.png)

## 各种小工具(tool)  

- `/hug|小泽抱|小泽抱抱|抱抱|抱抱小泽` 和小泽抱抱  
- `/名言警句` 获取本群网友的名人名言  
- `/全局名言警句` 获取随便一个群的名人名言  
- `/抽 <抽取人数>` 群抽奖小工具  
- 急急bot --被动触发，请自行探索

## 用户中心(uc)

!> 本模块处于测试阶段，如有问题请及时反馈。

<!-- TODO
- `/uc [info]` 进入用户中心
- `/uc gq <text>` 更新自己的个性签名(30字内)
- `/uc cancellation | /uc 销号` 彻底删除您在小泽中的所有信息 
-->  

- `/uc sign | /签到 | /sign` 每日签到

## 模块管理器(mm)  

**温馨提示：此模块尚未正式上线**  

- `/mm query <this|groupId|all> <moduleName|all>` 查询某模块在某处的启用状态
- `/mm set <this|groupId|all> <moduleName|all>` 设置某模块在某处的启用状态

## 管理命令  

!> 此类命令需要 [Bot协作者] 及以上权限。  

命令前缀：`~`  

- `zsay <text>` 让小泽说话
- `webapi <text>` 调用 WebMsgApi
- `boardcast <text>`  全体广播 **（高危）**
- `updatebcl` 立即更新云黑名单
- `updatectd` 立即更新 Cytoid 模块所有缓存
- `delallcache` 清理垃圾
- `setproxy` 重设代理地址
- `reload` 重载核心
- `screenshot` 截图

!> 本页面尚未完成，当前展示仅为预览版，不代表最终品质。  

*更新时间: 2022-8-8 23:11:14*
