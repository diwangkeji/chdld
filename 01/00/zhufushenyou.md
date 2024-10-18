# 祝福神油全新设置

<html xmlns="http://www.w3.org/1999/xhtml">
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
.hong {
	color: #F00;
}
.cheng {
	color: #F60;
}
.duanluo {
	padding-left: 4em;
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
/* code */
.code { background: #e5e5e5; padding: 10px 20px 10px; border: 1px solid #666; margin: 0; font-size: 16px; color:#333333;}
</style>
</head>

<body>
最后更新时间：2022/03/22<br />
<hr />


  <table width="200" height="100" border="1" cellpadding="0" cellspacing="0" bordercolor="#666" style="border-collapse:collapse;">
	<tr><td width="200" style="text-align: center">name</td><td width="100" style="text-align: center">Stdmode</td><td width="100" style="text-align: center">shape</td><td width="100" style="text-align: center">Weight</td><td width="100" style="text-align: center">looks</td><td width="100" style="text-align: center">DuraMax</td><td width="100" style="text-align: center">Ac</td></tr>
	<tr><td style="text-align: center">祝福神油</td><td style="text-align: center">3</td><td style="text-align: center">4</td><td style="text-align: center">1</td><td style="text-align: center">179</td><td style="text-align: center">1</td><td style="text-align: center">0</td></tr>
	<tr><td style="text-align: center">超级祝福神油</td><td style="text-align: center">3</td><td style="text-align: center">4</td><td style="text-align: center">1</td><td style="text-align: center">25899</td><td style="text-align: center">1</td><td style="text-align: center">1</td></tr>
  </table>
  <br />
  <span class="lan">相关设置：</span><br />
  <span class="duanluo"></span><span class="lan">AC1:设置0：普通祝福神油</span><br />
  <span class="duanluo"></span><span class="lan">AC1:设置1：超级祝福神油</span><br />
  <br />
<pre><div class="code">物品DB如下：

45;祝福神油;3;4;1;0;0;0;0;179;0;0;0;1;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;1000;10;0;0;0;0;8192
46;超级祝福神油;3;4;1;0;0;0;0;25899;0;0;0;1;0;0;0;0;1;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;1;10;0;0;0;0;0
</div></pre>
<br />
<hr />
<p class="biaoti">祝福神油使用触发</p>
<span class="cheng">1、使用祝福神油触发QF中 [@_祝福神油使用] 并返回以下参数</span><br /><br />
<span class="duanluo"></span><span class="zise">$PARAM(0) //使用对象 (主体/元神)</span><br />
<span class="duanluo"></span><span class="zise">$PARAM(1) //使用物品 (0:祝福神油 / 1:超级祝福神油)</span><br />
<span class="duanluo"></span><span class="zise">$PARAM(2) //使用状态 (0:成功 / 1:诅咒 / 2:失败)</span><br />
<br />

</body>
</html>
