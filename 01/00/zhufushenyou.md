# 祝福神油全新设置  

 最后更新时间：2022/03/22  

* * *

<table width="200" height="100" border="1" cellpadding="0" cellspacing="0" bordercolor="#666" style="border-collapse:collapse;"><tbody><tr><td width="200" style="text-align: center">name</td><td width="100" style="text-align: center">Stdmode</td><td width="100" style="text-align: center">shape</td><td width="100" style="text-align: center">Weight</td><td width="100" style="text-align: center">looks</td><td width="100" style="text-align: center">DuraMax</td><td width="100" style="text-align: center">Ac</td></tr><tr><td style="text-align: center">祝福神油</td><td style="text-align: center">3</td><td style="text-align: center">4</td><td style="text-align: center">1</td><td style="text-align: center">179</td><td style="text-align: center">1</td><td style="text-align: center">0</td></tr><tr><td style="text-align: center">超级祝福神油</td><td style="text-align: center">3</td><td style="text-align: center">4</td><td style="text-align: center">1</td><td style="text-align: center">25899</td><td style="text-align: center">1</td><td style="text-align: center">1</td></tr></tbody></table>

  
相关设置：  
AC1:设置0：普通祝福神油  
AC1:设置1：超级祝福神油  
  
```


物品DB如下：

45;祝福神油;3;4;1;0;0;0;0;179;0;0;0;1;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;1000;10;0;0;0;0;8192
46;超级祝福神油;3;4;1;0;0;0;0;25899;0;0;0;1;0;0;0;0;1;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;1;10;0;0;0;0;0



```
  

* * *

祝福神油使用触发

1、使用祝福神油触发QF中 \[@\_祝福神油使用\] 并返回以下参数  
  
$PARAM(0) //使用对象 (主体/元神)  
$PARAM(1) //使用物品 (0:祝福神油 / 1:超级祝福神油)  
$PARAM(2) //使用状态 (0:成功 / 1:诅咒 / 2:失败)