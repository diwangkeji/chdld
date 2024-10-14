<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=gb2312" />
<title>特殊标签分类</title>
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
}
.hong {
	color: #F00;
}
.duanluo {
	padding-left: 2em;
}
.zhushi {
	color: #0C0;
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
/* code */
.code { background: #e5e5e5; padding: 10px 35px 10px; border: 1px solid #666; margin: 0; font-size: 16px; color:#333333;}
</style>
</head>

<body>
最后更新时间：2022/03/22<br />
<hr />
<br />
<span class="biaoti">1、显示物品的图片和属性Tips</span><br /><br />
<span class="lan">&lt;/@@!PIC 物品名称&gt;</span><br /><br />
<pre><div class="code">[@示范]

&lt;/@@!PIC 圣战头盔&gt;      &lt;/@@!PIC 法神头盔&gt;     &lt;/@@!PIC 天尊头盔&gt;

</div></pre>
<br />

<span class="biaoti">2、显示指定的客户端图片</span><br /><br />
<span class="lan">&lt;@@!PIC2 packageID, 素材编号&gt;</span><br /><br />
<span class="zise">packageID：搜索说明书获取参数</span><br />
<br />
<pre><div class="code">[@示范]

&lt;@@!PIC2 3,15811&gt;  //显示客户端interface中15811号图片

</div></pre>
<br />

<span class="biaoti">3、自动行走到指定坐标</span><br /><br />
<span class="lan">&lt;/@@goplace 地图id 坐标X,坐标Y&gt;</span><br /><br />
<pre><div class="code">[@示范]

&lt;去将军坟东/@@goplace 0 775,400&gt;  //点击后人物会走到775:400坐标点

</div></pre>
<br />

<span class="biaoti">4、自动行走到指定坐标并打开NPC对话</span><br /><br />
<span class="lan">&lt;/@@goto 地图id NPC名字 坐标X,坐标Y&gt;</span><br /><br />
<span class="zise">说明：标签中X和Y的坐标点必须与NPC配置文本中的坐标点一样</span><br />
<br />
<pre><div class="code">[@示范]

&lt;去找落霞村铁匠/@@goto 1 铁匠 227,216&gt;  //点击后人物会走到227:216坐标点上打开铁匠对话框

</div></pre>
<br />

<span class="biaoti">5、文字颜色</span><br /><br />
<span class="lan">&lt;color=00ff00 彩虹独立端引擎&gt;</span><br /><br />
<pre><div class="code">[@示范]

&lt;color=00ff00 彩虹独立端引擎&gt;

{color=00ff00 &lt;$STR(S10)&gt;}

</div></pre>
<br />

<span class="biaoti">6、文字显示tips</span><br /><br />
<span class="lan">&lt;color=~显示文字信息#0xff00ff00 碰触显示&gt;</span><br /><br />
<pre><div class="code">[@示范]

&lt;color=~第一行文字信息#0xff00ff00$第二行文字信息#0xff00ff00$第三行文字信息#0xff00ff00 文字碰触显示&gt;

{color=~<$STR(S10)>#0xff00ff00$<$STR(S10)>#0xff00ff00$<$STR(S10)>#0xff00ff00 文字碰触显示}

</div></pre>
<br />

<span class="biaoti">7、点击标签显示文字tips</span><br /><br />
<span class="lan">&lt;color=~显示文字信息#0xff00ff00 碰触显示/@点击标签&gt;</span><br /><br />
<pre><div class="code">[@示范]

&lt;color=~第一行文字信息#0xff00ff00$第二行文字信息#0xff00ff00$第三行文字信息#0xff00ff00 进入地图/@进入地图&gt;

{color=~<$STR(S10)>#0xff00ff00$<$STR(S10)>#0xff00ff00$<$STR(S10)>#0xff00ff00 进入地图/@进入地图}

</div>
</pre>
<br />

</body>
</html>




