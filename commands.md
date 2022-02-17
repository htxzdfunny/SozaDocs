# 命令列表  

!> **注意:在阅读本文之前，请您务必先阅读[观前提示](./qa)。**  

## 基础命令( /z )  

- `/z` 存活测试
- `/z help` 调出帮助菜单
- `/z stat|status` 运行状态
- `小泽抱抱` 和小泽抱抱
- `/report <内容>` 问题反馈

## Cytoid信息查询( /ctd )  

特别鸣谢:Tigerhix Neo BillZhou233(冰糖酱) Sunset  

- `/ctd help` 调出模块菜单
- `/ctd ping` 检查伺服器连通性
- `/ctd bind <uid>` 绑定你的游戏账号
- `/ctd unbind` 无需参数，一键解绑账号
- `/ctd pf [uid|@]` 查询自己或他人的个人信息，如 rt/等级 等  
&nbsp;&nbsp;&nbsp;&nbsp;实例：`/ctd pf tigerhix` 查询 "tigerhix" 的个人信息  
- `/ctd info [uid|@] -q <N>` 查询自己或他人的最近第N条游玩记录(仅ranked mode，N≤10 且 ∈Z)*（开发中 可能不完善）*  
&nbsp;&nbsp;&nbsp;&nbsp;实例：`/ctd info miyou379 -q 2` 查询 "miyou379" 倒数第二条游玩记录  
&nbsp;&nbsp;&nbsp;&nbsp;`/ctd info -q 5` 查询绑定账号的倒数第五条游玩记录  
- `/ctd` --查询自己的最近游玩记录
- `/ctd set mode <image|text>` --切换图片/文字模式(仅对RecentPlay生效)*（开发中 可能不完善）*  
&nbsp;&nbsp;&nbsp;&nbsp;实例：`/ctd set mode image` 将您的默认输出模式改为图片模式  
&nbsp;&nbsp;&nbsp;&nbsp;![切换图片模式](https://cdn.u1.huluxia.com/g4/M01/25/68/rBAAdmG3QcCANSfLAAA0ypDCusc326.png)  

~~ 当然 存在概率性翻车的可能 ~~  

&nbsp;&nbsp;&nbsp;&nbsp;![翻车了](https://cdn.u1.huluxia.com/g4/M03/25/69/rBAAdmG3Qi2AeHWiAABp2Lsn_ww173.png)  

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

## 音游狗老黄历

来自 [@mugtungshing_bot](https://t.me/mugtungshing_bot)  

> 热知识：你知道吗？老黄历中的人品值是由 Dice 骰娘网络下发的
![某Dice文档](https://p0.meituan.net/csc/a5756f2f388bb0ee804d1701782600855858.png)  
[图片来源](https://v2docs.kokona.tech/zh/latest/User_Manual.html?highlight=jrrp#jrrp)

- `@小泽 /today` 查询您的今日黄历  
实例：

![老黄历](https://cdn.u1.huluxia.com/g4/M03/25/73/rBAAdmG3R-yABPS1AAA9irZXntI887.png)

!> 请注意：请不要复制别人的命令，这会导致消息中的 at 码转为普通文本，将无法被小泽识别。  

## 名言警句

- `/名言警句` 获取一句群友的名言警句 *需要联系开发者手动添加*
- `/全局名言警句` 随机获取所有群中某个网友的怪话  

## 环保排行榜  

（其实就是个计草器 还不准）  

- `/GR` 查看全局环保排行榜  
- `/GR -g` 查看本群环保排行榜  

## 图片生成  

### 基本玩法

- `致电<名称> <@某人>` 致电某人
- `高情商 <内容> 低情商 <内容>` 高低情商
- `捏<我|QQ|at>` 捏捏头像  

除此以外，还有一些进阶玩法：  

### 调用 PlantUML 绘图  

[PlantUML中文用户手册](https://plantuml.com/zh/guide)  
注：如果您是普通用户想要尝试，除非您真的很有耐心，否则还请您移步搜索引擎搜索 `PlantUML快速入门` ，因为这本手册极度详细，目前有 398 页（

使用例子如下：  

```
@startuml
Alice -> Bob: test
@enduml
```

![实例](https://p1.meituan.net/csc/7cfe10d9f3771cbdb6b5e7c4286e707e12538.png)

## 管理命令  

!> 此类命令需要 [Bot协作者] 及以上权限。  

命令前缀：`~`  

- `zsay <text>` 让小泽说话
- `webapi <text>` 调用 WebMsgApi
- `boardcast <text>`  全体广播（高危）
- `updatebcl` 立即更新 Dice! 云黑名单
- `updatectd` 立即更新 Cytoid 模块所有缓存
- `delallcache` 清理垃圾

!> 本页面尚未完成，当前展示仅为预览版，不代表最终品质。  
