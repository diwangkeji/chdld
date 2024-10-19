# 祝福油罐说明  

最后更新时间：2022/03/22

* * *


| **name** | **Stdmode** | **shape** | **Anicount** | **looks** | **DuraMax** |
|----------|-------------|-----------|--------------|-----------|-------------|
| **祝福油罐** | 37          | 210       | 24           | 1047      | 50          |



  
```
物品完整DB：

323;祝福油罐;37;210;1;24;1;0;0;1047;0;0;0;50;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;0;40000;5;0;0;0;0;532864

```
  
对应触发脚本  

```
[@StdModeFunc24]
#IF
EQUAL $ITEMINFO[$PARAM(1)].NAME
!CHECKBAGSIZE 1
#ACT
SENDMSG 5 包裹空位不足！
break
#IF
EQUAL $ITEMINFO[$PARAM(1)].NAME 
SMALL $ITEMINFO[$PARAM(0)].AC1 1
#ACT
SENDMSG 5 祝福油灌中没有存放祝福神油！
break
#IF
EQUAL $ITEMINFO[$PARAM(1)].NAME 
LARGE $ITEMINFO[$PARAM(0)].AC1 0
#ACT
UPGRADEUSERITEM $PARAM(0) 4 - 1
UPGRADEUSERITEM $PARAM(0) 1 - 1
GIVE 祝福神油 1
break
#IF
EQUAL $ITEMINFO[$PARAM(0)].NAME 祝福油罐
EQUAL $ITEMINFO[$PARAM(1)].NAME 祝福神油
EQUAL $ITEMINFO[$PARAM(0)].AC1 $ITEMINFO[$PARAM(0)].DURAMAX
#ACT
SENDMSG 5 你的祝福油罐无法容纳更多祝福神油
break
#IF
EQUAL $ITEMINFO[$PARAM(0)].NAME 祝福油罐
EQUAL $ITEMINFO[$PARAM(1)].NAME 祝福神油
SMALL $ITEMINFO[$PARAM(0)].AC1 $ITEMINFO[$PARAM(0)].DURAMAX
#ACT
UPGRADEUSERITEM $PARAM(0) 4 + 1
TAKEM $PARAM(1)
break

```