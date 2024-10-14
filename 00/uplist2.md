
<html>
<head>
<meta http-equiv="Content-Type" content="text/html; charset=gb2312" />
<style type="text/css">
body {
	margin-left: 50px;
	margin-top: 50px;
	margin-right: 50px;
	margin-bottom: 50px;
	color: #000;
}
.zise {
	color: #90F;
}
.lan {
	color: #00F;
}
.fen {
	color: #F0F;
	font-weight: bold;
}
.hong {
	color: #F00;
	font-weight: bold;
}
.duanluo {
	padding-left: 2em;
}
.zhushi {
	color: #007700;
	font-weight: bold;
}

.biaoti {
	font-weight: bold;
	font-size: 24px;
	color: #F0F;
}
.cheng {
	color: #F60;
	font-weight: bold;
}

.url {
	color: #F0F;
	font-size: 20px;
	font-weight: bold;
}

/* code */
.code { background: #e5e5e5; padding: 10px 20px 10px; border: 1px solid #666; margin: 0; font-size: 14px; color:#333333;}
</style>
</head>

<body>
最后更新时间：2022/07/09<br />
<hr />

<pre><div class="code"><span class="cheng">0728引擎修复日志</span>

1、修正加载MapQuest.txt地图任务脚本异常的问题;

2、修正INCHP地图属性参数异常的问题;

3、修正装备穿戴不计算攻击加成的问题;

4、修正自动打怪状态使用治疗术异常的问题;

5、修正自动打怪状态使用施毒术/强化施毒术异常的问题;

6、修正$WOLTIMETODATETIME(X)变量返回日期错误的问题;

7、修正服务端ShieldProp.Xml配置无效的问题;

8、修正人物跑动时打开技能面板停止的问题;

9、修正“神圣腰带”特殊属性异常的问题;

10、修正玩家追杀画面同步异常的问题;

11、修正游戏多开客户端资源下载异常的问题;

12、修正客户端系统设置PK保护无法使用随机神石的问题;

13、修正神秘灵匣服务端配置修改ui后无法读取指定界面的问题;

<span class="hong">本次其他程序更新</span>

1、更新GameCenter.exe程序，丰富定时任务，新增数据维护备份游戏数据

2、运行GameCenter.exe后自动生成gzip.exe程序为正常现象

3、更新DBServer.exe程序

<span class="hong">本次引擎更新事项</span>

1、服务端 sql\bin 文件目录中，需添加 mysqldump.exe 程序，可在程序压缩包中获取

</div></pre>
<br />

<pre><div class="code"><span class="cheng">0709引擎修复日志</span>

1、修正行会攻击模式无法攻击敌对行会宠物的问题;

2、修正抗拒火环设置卡位时间不卡位的问题;

3、修正自动突斩、自动野蛮推人异常的问题;

4、修正怒斩天下技能无法设置特效的问题;

5、修正调整元神体魄不刷新排行榜的问题;

6、修正绿毒不触发吸血的问题;

7、修正元神执行SETWEAPONGROW / SETWINGGROW 命令无效的问题;

8、修正UseBonusPoint命令增加HP过地图异常的问题;

9、修正两种不同叠加物品拖拽触发叠加效果的问题;

10、修正施毒术释放后目标立即掉血的问题;

11、修正神光术无法解除麻痹的问题;

12、修正标签tips显示异常的问题;

13、修正5710特效异常的问题;

14、修正SETUSERITEMSTR命令保存数据异常的问题;

15、新增道士自动打怪界面设置召唤技能选项;

16、新增人物佩戴“瞬移戒指”后，可在寻路界面双击自动传送;

</div></pre>
<br />

<pre><div class="code"><span class="cheng">0516引擎修复日志</span>

1、修正引擎面板吸血值调整为0不保存的问题;

2、修正商城无法购买1元宝物品的问题;

3、修正MOV赋值异常的问题;

4、修正getexp命令异常的问题;

5、新增范围拾取规则

      引擎参数位置：
      引擎面板 -> 选项 -> 参数设置 -> 装备掉落 -> 范围拾取规则

<span class="hong">本次引擎更新事项</span>

1、更新 GameLoad DB Manager.exe工具，扩展物品数据库支持勾选“禁止范围拾取”

</div></pre>
<br />



<pre><div class="code"><span class="cheng">0510引擎修复日志</span>

1、修正自定义货币不刷新的问题;

2、修正自定义货币无法购买商城物品的问题;

3、修正装备强化未返回祝福石ID的问题;

4、修正集中刷怪后无法推动怪物的问题;

5、修正离线挂机后登录攻速异常的问题;

6、修正翱风斩技能特效错误的问题;

7、修正调整人物职业后自动打怪页面不刷新的问题;

8、修正宝宝杀怪$KILLMONNAME不刷新的问题;

9、调整引擎参数中“申请行会费用”、“申请行会战费用”数值可为0

<span class="hong">本次引擎【MagicSkill.xml】调整(用户需设置以下参数)</span>

1、“火毒攻心剑”技能新增Value9为地面特效(0/1/2)

2、“神之召唤”技能新增Value5为怪物攻击倍数(默认100)

3、“毒凌波”技能新增Value15为怪物掉血最大值。Value6为人物掉血最大值

<span class="hong">本次引擎更新事项</span>

1、本次更新游戏网关，支持移动速度参数设置！请删除游戏网关配置，由网关自动生成新的封挂参数

    <span class="hong">0510网关免费激活码：FP8G-844K-CNRA-N6FX</span>

2、更新 GameLoad DB Manager.exe工具，扩展GameLoad.DB数据库对应“打怪伤害加成”、“移动速度”、“范围拾取”

</div></pre>
<br />





<pre><div class="code"><span class="cheng">0422引擎修复日志</span>

1、修正飞行靴界面无法勾选的问题;

2、修正打宝特权经验无法超255的问题;

3、修正MONEY货币不保存的问题;

4、修正魔法盾技能特效异常的问题;

5、修正强化火球术技能效果异常的问题;

6、修正怒斩天下技能伤害错误的问题;

7、修正人物上线能立即释放烈火剑法/雷霆剑的问题;

8、修正离线挂机登录活力值、特权物品不显示的问题;

9、修正SENDMSG飘红冲突的问题;

10、修正人物中毒宝宝不转移分担伤害的问题;

11、修正宠物杀怪不触发MapQuest的问题;

12、调整施毒术掉血点数与人物幸运值挂钩;

13、调整火毒攻心剑技能XML参数8为中毒时间;

14、调整雪莲类、神水类药品支持need、needlevel使用需求检测;

15、调整抗性属性可作用毒凌波技能掉血;

<span class="hong">本次引擎【物品DB】调整(用户需设置以下参数)</span>

神秘钥匙    stdmode:37   shape:208    DuraMax:1
神秘钥匙串  stdmode:37   shape:208    DuraMax:20
解除神水    stdmode:3    shape:13     DuraMax:1
随机神石    stdmode:3    shape:19     DuraMax:128

<span class="hong">本次引擎【技能DB】调整(用户需设置以下参数)</span>

怒斩天下    Job:4
天怒惊雷    Job:5
天女散花咒  Job:6
迷光烈焰    Job:7
火毒攻心剑  Job:8
神之召唤    Job:9

<span class="hong">本次引擎更新事项</span>

1、本次引擎需要更新sql文件，用户需替换配套程序中sql文件夹，否则报错！

2、本次扩展数据库，老测试用户使用工具删除woool_game老数据库，具体操作可参考说明书

3、本次更新游戏网关，攻速+10支持无限刀不卡顿！请删除游戏网关配置，由网关自动生成新的封挂参数

</div>
</pre>
<br />

</body>
</html>
