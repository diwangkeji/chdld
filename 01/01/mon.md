# 怪物数据库字段说明


<html>
<head>
<meta http-equiv="Content-Type" content="text/html; charset=gb2312" />
<style type="text/css">
body,td,th {
	color: #000;
}
body {
	margin-left: 50px;
	margin-top: 50px;
	margin-right: 50px;
	margin-bottom: 50px;
	color: #666;
}
.zise {
	color: #90F;
}
.lan {
	color: #00F;
}
.fen {
	color: #F0F;
}
.hong {
	color: #F00;
}
.duanluo {
	padding-left: 3em;
}
.zhushi {
	color: #0C0;
	font-weight: bold;
}

.biaoti {
	font-weight: bold;
	font-size: 24px;
	color: #F0F;
}
</style>
</head>

<body>
最后更新时间：2022/03/22<br />
<hr />


  <span class="lan">警告！<br />
DC和DCMAX设置时禁止500-500、500-300这样的设置，否则会出现秒杀！ 
<br />
MC和SC设置时禁止500-500、500-300这样的设置，否则会出现秒杀！ 
<br />
必须按照前低后高的格式设置！</span><br />
<br />
<table width="500" height="1024" border="1" cellpadding="0" cellspacing="0" bordercolor="#666" style="border-collapse:collapse;">
  <tr style="height:40px; width:250"><td width="200">字段名字</td>
    <td width="200">说明1</td>
    <td width="200">说明2</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>Name</td>
    <td>怪物名字 </td>
    <td nowrap="nowrap">设置怪物名时，禁止使用( )括号，可使用全半角字符代替，比如：白蛇妖·精</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>Race</td>
    <td>怪物攻击类型</td>
    <td>&nbsp;</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>Racelmg</td>
    <td>怪物攻击效果</td>
    <td>&nbsp;</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>Appr</td>
    <td>怪物外观</td>
    <td>&nbsp;</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>Lvl</td>
    <td>怪物等级</td>
    <td>&nbsp;</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>Undead</td>
    <td>0-7表示不同等级的诱惑之光可诱惑的怪物;<br />
      254为BOSS怪,不可被诱惑和圣言杀死;<br />
    255为该怪不可被诱惑但可以被圣言杀死;</td>
    <td nowrap="nowrap">补充：<br />
      诱惑之光与圣言术额外设置可参考最新MagicSkill.xml进行设置;<br />
    心魔类怪物Undead=2表示主动攻击;</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>CoolEye</td>
    <td>设置怪物反隐身、反替身</td>
    <td><p>设置范围：<br />
      0 //不反隐身、不反替身；<br />
      1 //反隐身；<br />
      2 //反替身；<br />
    3 //反隐身、反替身；</p></td>
  </tr>
  <tr style="height:40px; width:250">
    <td>ViewRange</td>
    <td>怪物视野范围</td>
    <td>&nbsp;</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>EXP</td>
    <td>怪物的经验值</td>
    <td>&nbsp;</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>HP</td>
    <td>怪物生命值</td>
    <td>最高支持21亿</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>MP</td>
    <td>怪物魔法值</td>
    <td>最高支持21亿</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>AC</td>
    <td>怪物防御值</td>
    <td>最高支持21亿</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>MAC</td>
    <td>魔法防御值</td>
    <td>最高支持21亿</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>DC</td>
    <td>攻击力</td>
    <td>最高支持21亿</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>DCMAX</td>
    <td>最大攻击力</td>
    <td>最高支持21亿</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>MC</td>
    <td>魔法攻击力</td>
    <td>&nbsp;</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>SC</td>
    <td>道术攻击力</td>
    <td>&nbsp;</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>SPEED</td>
    <td>躲避</td>
    <td>&nbsp;</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>HIT</td>
    <td>命中</td>
    <td>&nbsp;</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>Walk_SPD</td>
    <td>行走速度(时间单位：毫秒)</td>
    <td>&nbsp;</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>WalkStep</td>
    <td>行走步伐</td>
    <td>默认1</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>WalkWait</td>
    <td>行走等待(时间单位：毫秒)</td>
    <td>数字越大,下次攻击间隔越长</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>ATTACK_SPD</td>
    <td>攻击速度(时间单位：毫秒)</td>
    <td>数字越大,下次攻击间隔越长</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>SPCode</td>
    <td>特殊属性</td>
    <td>&nbsp;</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>BURST</td>
    <td nowrap="nowrap">此字段为Envir\MonItems目录下的指定暴率文件<br />
名，不包含.txt后缀</td>
    <td nowrap="nowrap">不使用镜像爆率时，此字段请留空，不要填任何内容。</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>NameColor</td>
    <td>怪物名字颜色(0-255)</td>
    <td>&nbsp;</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>AI</td>
    <td>保存怪物：变身/复活、附加效果</td>
    <td>&nbsp;</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>Tenacity</td>
    <td>韧性(抵抗暴击)</td>
    <td>&nbsp;</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>SDC</td>
    <td>神圣攻击下限</td>
    <td>&nbsp;</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>SDCMAX</td>
    <td>神圣攻击上限</td>
    <td>&nbsp;</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>ElementDC1</td>
    <td>金攻击</td>
    <td>最高支持65535</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>ElementDC2</td>
    <td>木攻击</td>
    <td>最高支持65535</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>ElementDC3</td>
    <td>土攻击</td>
    <td>最高支持65535</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>ElementDC4</td>
    <td>水攻击</td>
    <td>最高支持65535</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>ElementDC5</td>
    <td>火攻击</td>
    <td>最高支持65535</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>ElementAC1</td>
    <td>金防御</td>
    <td>最高支持65535</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>ElementAC3</td>
    <td>木防御</td>
    <td>最高支持65535</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>ElementAC4</td>
    <td>土防御</td>
    <td>最高支持65535</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>ElementAC5</td>
    <td>水防御</td>
    <td>最高支持65535</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>ElementAC5</td>
    <td>火防御</td>
    <td>最高支持65535</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>MilitaryExp</td>
    <td>功勋值</td>
    <td>&nbsp;</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>RepressDemonExp</td>
    <td>镇魔珠经验</td>
    <td>&nbsp;</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>Thump </td>
    <td>暴击</td>
    <td>&nbsp;</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>ReduceAC</td>
    <td>减免防御</td>
    <td>&nbsp;</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>ReduceAvoid</td>
    <td>减免躲避</td>
    <td>&nbsp;</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>SacredDamReduceLv</td>
    <td>神圣免伤等级</td>
    <td>&nbsp;</td>
  </tr>
  <tr style="height:40px; width:250">
    <td>PoisonNicety</td>
    <td>中毒命中</td>
    <td>&nbsp;</td>
  </tr>
</table>
</body>
</html>
