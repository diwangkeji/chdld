 # 魂珠物品相关设置
 
 最后更新时间：2022/03/22  

* * *

魂珠物品DB设置

| **name** | **Stdmode** | **shape** | **Anicount** | **looks** | **DuraMax** |
|----------|-------------|-----------|--------------|-----------|-------------|
| **真魂珠**  | 13          | 1         | 0            | 30567     | 1           |


  
```
物品完整DB：

666;真魂珠;13;1;1;0;0;0;0;30576;0;65;0;1;100;100;100;0;10;10;10;10;10;10;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0
667;仙魂珠;13;2;1;1;0;0;0;30577;0;65;0;1;200;200;200;0;20;20;20;20;20;20;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0

```

魂珠经验设置

魂珠经验根据物品DB中Anicount的值对应读取服务端配置文件 "Mir200\\Config\\ItemCfg.ini"中的数据  
  
```
[SoulBead0]              ;//表示Anicount为0的魂珠读取
SoulBeadMaxLevel=10      ;//表示魂珠提升最高等级
Level1=240000000
Level2=600000000
Level3=1050000000
Level4=1800000000
Level5=2700000000
Level6=5400000000
Level7=6900000000
Level8=8400000000
Level9=12000000000
Level10=18000000000

[SoulBead1]              ;//表示Anicount为1的魂珠读取
SoulBeadMaxLevel=10      ;//表示魂珠提升最高等级
Level1=20200000000
Level2=26200000000
Level3=30000000000
Level4=33000000000
Level5=36000000000
Level6=40000000000
Level7=43000000000
Level8=46000000000
Level9=50000000000
Level10=60000000000


```

魂珠升级经验开关

引擎面板 -> 选项 -> 参数设置 -> 升级经验 -> 勾选【佩戴魂珠主体不加经验】  
  

魂珠相关命令

1、调整物品当前经验值命令  
  
UPGRADEITEMEXP 参数1 参数2 参数3  
  
参数1： 物品ID  
参数2： 操作符(+、 -、 =)  
参数3： 数值  
  
```


[@测试脚本]
#IF
True
#ACT
give 真魂珠 1
UPGRADEITEMEXP $PARAM(10) + 1000
SENDMSG 5 真魂珠增加1000点蕴藏经验
break
```
  
2、变量返回  
  
```
$ITEMINFO[X].EXP             ;//X:物品ID，返回物品当前经验值

$ITEMINFO[X].SOULBEADMAXEXP  ;//X:物品ID，返回魂珠物品最大经验值

```