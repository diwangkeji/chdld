 # 怪物Race对照表 
 
最后更新时间：2022/05/10  

* * *

  <table width="900" height="900" border="1" cellpadding="0" cellspacing="0" bordercolor="#666" style="border-collapse:collapse;">
  <tr><td width="200" style="text-align: center">攻击代码</td><td width="500">说明</td><td width="500">怪物/功能</td></tr>
  <tr>
    <td style="text-align: center">11</td>
    <td width="500">无敌加瞬移攻击，主动攻击MOB和红人</td>
    <td width="500">卫士</td>
  </tr>
  <tr>
    <td style="text-align: center">12</td>
    <td width="500">自动寻路怪物，终点消失时，将触发机器人脚本[@离火封魔阵]</td>
    <td width="500">离火封魔阵</td>
  </tr>
  <tr>
    <td style="text-align: center">13</td>
    <td width="500">不会攻击红名和宝宝</td>
    <td width="500">公主侍卫</td>
  </tr>
  <tr>
    <td style="text-align: center">14</td>
    <td width="500">近身攻击自动寻路怪物类型</td>
    <td width="500">离火封魔阵</td>
  </tr>
  <tr>
    <td style="text-align: center">15</td>
    <td width="500">不走动，卫士不攻击，被攻击不会还击</td>
    <td width="500">矿石资源</td>
  </tr>
  <tr>
    <td style="text-align: center">17</td>
    <td width="500">不会攻击，只会躲闪</td>
    <td width="500">天玉公主</td>
  </tr>
  <tr>
    <td style="text-align: center">18</td>
    <td width="500">设置被吃的物品，请把物品的looks，填入怪物DB的MP字段里</td>
    <td width="500">贪吃的霸王鱼<br /></td>
  </tr>
  <tr>
    <td style="text-align: center">20</td>
    <td width="500">不主动攻击，不会移动，远程攻击</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">21</td>
    <td width="500">远程攻击自动寻路怪物类型</td>
    <td width="500">离火封魔阵</td>
  </tr>
  <tr>
    <td style="text-align: center">22</td>
    <td width="500">自身不移动，只能使用伐木斧。</td>
    <td width="500">树</td>
  </tr>
  <tr>
    <td style="text-align: center">23</td>
    <td width="500"><p>可采集怪物类型：<br />
      　
      AC为采集时间；<br />
      　
      MAC为采集完成后怪物是否消失，(0:不消失，1:消失)；<br />
      　
      DCMAX为设置触发标签专属ID；<br />
      　
      DC   设置采集后冷却时间，单位(秒)；</p>
      <p>2)、玩家点击采集怪物触发QF脚本 [@采集开始_X] X为触发ID，并返回以下参数<br />
        　
        $PARAM(0)   //采集怪物名字<br />
        　
        $PARAM(1) //采集怪物ID<br />
        　
        $PARAM(2) //采集剩余倒计时(秒)</p>
      <p>3)、新增命令 StartCollect A 为玩家开始进行采集<br />
        　
        A: 怪物ID</p>
      <p>4)、新增变量 $CollectionID 为当前玩家正在采集的怪物ID</p>
      <p>5)、玩家采集结束触发QF脚本 [@采集结束_X] X为触发ID，并返回以下参数<br />
        　
        $PARAM(0) //采集怪物名字</p>
      <p>6)、新增命令 RESETCOLLMONTIME 为初始化采集冷却时间</p>
      <p>//此命令用于采集结束后，初始化该采集怪物冷却时间</p>
      <p>[@采集结束_1]<br />
        #IF<br />
        !CHECKITEM $PARAM(0)   1<br />
        #ACT<br />
        RESETCOLLMONTIME<br />
        give 一朵鲜花 1<br />
        SENDMSG 5   恭喜勇士获得一朵鲜花!<br />
    break</p></td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">51</td>
    <td width="500">可以挖的类型，低品质</td>
    <td width="500">兔、癞蛤蟆、鹿</td>
  </tr>
  <tr>
    <td style="text-align: center">52</td>
    <td nowrap="nowrap">灵兽类、座骑类；可以挖的类型，高品质</td>
    <td width="500">猪、牛、丛林豹、踏云豹等等</td>
  </tr>
  <tr>
    <td style="text-align: center">53</td>
    <td width="500">主动攻击；可以挖的类型</td>
    <td width="500">蝎子、土狼</td>
  </tr>
  <tr>
    <td style="text-align: center">54</td>
    <td width="500">只会逃跑类型</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">55</td>
    <td width="500">练功师</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">56</td>
    <td width="500">捕捉灵兽怪物类型</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">80</td>
    <td width="500">被动近身攻击</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">81</td>
    <td width="500">对象进入范围主动攻击</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">82</td>
    <td width="500">2格攻击范围内毒液攻击-弱；可以挖的类型</td>
    <td width="500">毒蜘蛛</td>
  </tr>
  <tr>
    <td style="text-align: center">83</td>
    <td width="500">出生自带特效AI，近战攻击！</td>
    <td nowrap="nowrap">幽影武士、幽影骑士 Race：83 Appr：225、548、741 //带出生动画近身攻击；<br />
      新尸王：Race：83 Appr：533   //带出生动画近身攻击；<br />
    新尸王：Race：83 Appr：547 //带出生动画近身攻击；</td>
  </tr>
  <tr>
    <td style="text-align: center">84</td>
    <td width="500">主动近身攻击</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">85</td>
    <td width="500">地下钻出来，原地攻击，死后物品不掉落；可以挖的类型</td>
    <td width="500">食人花</td>
  </tr>
  <tr>
    <td style="text-align: center">86</td>
    <td width="500">主动近身攻击</td>
    <td width="500">尸卫</td>
  </tr>
  <tr>
    <td style="text-align: center">87</td>
    <td width="500">主动攻击射程5</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">88</td>
    <td width="500">主动近身物理攻击</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">89</td>
    <td width="500">主动近身物理攻击</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">90</td>
    <td width="500">近身麻痹攻击,几率低；可以挖的类型</td>
    <td width="500">洞蛆</td>
  </tr>
  <tr>
    <td style="text-align: center">91</td>
    <td width="500">主动近身攻击</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">92</td>
    <td width="500">设置为物品刷出来后自动掉落</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">93</td>
    <td width="500">边攻击边躲避</td>
    <td width="500">烈焰使</td>
  </tr>
  <tr>
    <td style="text-align: center">94</td>
    <td width="500">主动攻击、直线攻击</td>
    <td width="500">僵尸</td>
  </tr>
  <tr>
    <td style="text-align: center">95</td>
    <td width="500">对象进入攻击范围内会从地下爬出来</td>
    <td width="500">僵尸</td>
  </tr>
  <tr>
    <td style="text-align: center">96</td>
    <td width="500">死亡后自动复活一次</td>
    <td width="500">僵尸</td>
  </tr>
  <tr>
    <td style="text-align: center">97</td>
    <td width="500">近身魔法攻击</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">98</td>
    <td width="500">近身攻击</td>
    <td width="500">海妖狂战士、炎魔</td>
  </tr>
  <tr>
    <td style="text-align: center">99</td>
    <td width="500">会推开周围玩家</td>
    <td width="500">驭冰游神</td>
  </tr>
  <tr>
    <td style="text-align: center">100</td>
    <td width="500">道士宝宝变异骷髅专属AI</td>
    <td width="500">变异骷髅</td>
  </tr>
  <tr>
    <td style="text-align: center">101</td>
    <td width="500">进入范围会从石像状态激活</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">102</td>
    <td width="500">可召唤怪物，在mir200\Envir\MonsterChild.txt进行相关设置</td>
    <td width="500">逆魔之王</td>
  </tr>
  <tr>
    <td style="text-align: center">103</td>
    <td width="500">自身不移动，通过mir200\Envir\MonsterChild.txt设置的怪物攻击目标</td>
    <td width="500">蚁巢</td>
  </tr>
  <tr>
    <td style="text-align: center">104</td>
    <td width="500">主动攻击，射程8</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">105</td>
    <td width="500">麻痹石化攻击；可以挖的类型</td>
    <td width="500">铁翼魔</td>
  </tr>
  <tr>
    <td style="text-align: center">106</td>
    <td width="500">麻痹石化攻击；可以挖的类型</td>
    <td width="500">闪电魔</td>
  </tr>
  <tr>
    <td style="text-align: center">107</td>
    <td width="500">机关巨兽</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">108</td>
    <td width="500">可召唤怪物，在mir200\Envir\MonsterChild.txt进行相关设置</td>
    <td width="500">逆魔</td>
  </tr>
  <tr>
    <td style="text-align: center">109</td>
    <td width="500">远程魔法攻击</td>
    <td width="500">碧血魔</td>
  </tr>
  <tr>
    <td style="text-align: center">110</td>
    <td width="500">沙城城门</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">111</td>
    <td width="500">皇宫左、中、右墙</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">112</td>
    <td width="500">只主动攻击红名，射程11</td>
    <td width="500">弓箭守卫</td>
  </tr>
  <tr>
    <td style="text-align: center">113</td>
    <td width="500">道士宝宝火灵珠专属AI</td>
    <td width="500">火灵珠： race=113， raceimg=54， appr=110</td>
  </tr>
  <tr>
    <td style="text-align: center">114</td>
    <td width="500">道士宝宝麒麟专属AI<br /></td>
    <td width="500">麒麟： race=114 ，raceimg=55 ，appr=111</td>
  </tr>
  <tr>
    <td style="text-align: center">115</td>
    <td width="500">禁地魔王，数据库 Mc - Sc 为禁地魔王释放红毒所减少防御魔防值</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">116</td>
    <td width="500">自身不移动，通过mir200\Envir\MonsterChild.txt设置的怪物攻击目标</td>
    <td width="500">幽灵虫母</td>
  </tr>
  <tr>
    <td style="text-align: center">117</td>
    <td width="500">自身没有攻击力，通过自暴来攻击对象</td>
    <td width="500">幽灵虫</td>
  </tr>
  <tr>
    <td style="text-align: center">118</td>
    <td width="500">隔一格攻击，主动移动攻击</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">119</td>
    <td width="500">为近身、或隔位附带绿毒攻击</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">120</td>
    <td width="500">无敌，不移动，不攻击</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">121</td>
    <td width="500">自身不移动，通过mir200\Envir\MonsterChild.txt设置的怪物攻击目标</td>
    <td width="500">寒荒海兽</td>
  </tr>
  <tr>
    <td style="text-align: center">122</td>
    <td width="500">逆魔卫士</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">123</td>
    <td width="500">逆魔雕像</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">124</td>
    <td width="500">逆魔弓箭手</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">125</td>
    <td width="500">逆魔侍卫</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">126</td>
    <td nowrap="nowrap">对攻击目标有火墙攻击效果，并且当目标进入4格范围内时，将会把攻击目标推开;<br />
    DC=火墙的最低攻击力<br />
    DcMax=火墙的最高攻击力</td>
    <td width="500">调皮小鬼</td>
  </tr>
  <tr>
    <td style="text-align: center">127</td>
    <td width="500">攻击范围由ViewRange决定</td>
    <td width="500">魔眼</td>
  </tr>
  <tr>
    <td style="text-align: center">128</td>
    <td width="500">近身火墙攻击<br />
    DC=火墙的最低攻击力<br />
    DcMax=火墙的最高攻击力</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">129</td>
    <td width="500">使用六大神技：狂潮飞刺、召唤魔炎、横扫千军、退敌魔咒、怒震山河、移形换位<br />
    物理攻击使用DC-MAXDC ，地面魔炎攻击力使用MC- SC</td>
    <td width="500">铁血魔王</td>
  </tr>
  <tr>
    <td style="text-align: center">130</td>
    <td width="500">道士宝宝烈焰麒麟、怒焰麒麟专属AI，魔法攻击使用DC- MAXDC设置攻击力<br /></td>
    <td width="500">烈焰麒麟： race=130，raceimg=55 ，appr=342<br />
    怒焰麒麟： race=130，raceimg=55 ，appr=343</td>
  </tr>
 
  <tr>
    <td style="text-align: center">131</td>
    <td width="500">暗影雷电类型怪物</td>
    <td width="500">        AC：怪物预警特效 (可参考magicfile特效)<br />
        MAC：怪物攻击特效 (可参考magicfile特效)<br />
        DC：攻击下限<br />
        DCMAX：攻击上限<br />
        MC：当DC和DCMAX为0时，则MC为怪物攻击百分比掉血<br />
        SC：伤害范围<br />
        WALKWAIT：预警时间(毫秒)<br />
        ATTACK_SPD：攻击间隔(毫秒)<br /></td>
  </tr>

  <tr>
    <td style="text-align: center">132</td>
    <td width="500">道士宝宝骷髅战士专属AI，双头暴熊</td>
    <td width="500">骷髅战士：race=132，raceimg=55， appr=429</td>
  </tr>
  <tr>
    <td style="text-align: center">133</td>
    <td width="500">道士宝宝骷髅法师专属AI</td>
    <td width="500">骷髅法师：race=133，raceimg=55， appr=430</td>
  </tr>
  <tr>
    <td style="text-align: center">134</td>
    <td width="500">通天教主、阿修罗神 </td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">135</td>
    <td width="500">可召唤怪物，在mir200\Envir\MonsterChild.txt进行相关设置</td>
    <td width="500">啸天虎妖<br /></td>
  </tr>
  <tr>
    <td style="text-align: center">136</td>
    <td width="500">可召唤怪物，在mir200\Envir\MonsterChild.txt进行相关设置</td>
    <td width="500">无相天魔</td>
  </tr>
  <tr>
    <td style="text-align: center">137</td>
    <td width="500">Mc - Sc控制加血值</td>
    <td width="500">黑袍修罗</td>
  </tr>
  <tr>
    <td style="text-align: center">138</td>
    <td width="500">黑袍修罗长老，Mc - Sc控制加血值<br />
      可直接使用MonGen.txt刷新长老，格式如下：//实现与官方一致长老阵系统<br />
      AS004 233 63   黑袍修罗长老 20 40 25<br />
    AS004 218 76 黑袍修罗长老 20 20 25</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">139</td>
    <td width="500">对直线5个坐标造成伤害。<br />
      DC - MAXDC:是物理伤害 <br />
      MC -   SC:是魔法伤害(可用于魔斗士)<br />
      //当139作用于魔神修罗，攻击坐标为2格<br />
    //当139作用于炎魔，攻击坐标为3格</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">140</td>
    <td width="500"><p>深渊领主AI<br />
      //实现赤血魔弑、君临天下、嗜焱焚天、魔神降临、枯骨禁魂、魔君召令技能<br />
      //第一形态死亡不增加经验，不掉落物品。需要在数据库设置死亡后1秒变身第二形态<br />
      //可召唤怪物，在mir200\Envir\MonsterChild.txt进行相关设置</p></td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">142</td>
    <td width="500">魔化沙兽、铁血刺客：Race：142 RaceImg：17</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">143</td>
    <td width="500">忧之心魔：Race：143 RaceImg：17<br />
      喜之心魔：Race：143 RaceImg：18<br />
      思之心魔：Race：143   RaceImg：19<br />
      悲之心魔：Race：143 RaceImg：20<br />
      惊之心魔：Race：143   RaceImg：21<br />
      怒之心魔：Race：143 RaceImg：22<br />
      恐之心魔：Race：143 RaceImg：23   ;//此怪物AI会召唤一只宠物协助作战，可在mir200\Envir\MonsterChild.txt进行设置！<br />
      <p>以上心魔攻击都会追击15个坐标，超过15个坐标则会自己返回刷新点！但需要使用以下命令来刷出心魔怪物。<br />
        如果刷出坐标不在集中点坐标，则怪物刷出后，会走到集中点坐标上</p>
      <p>[@示范]<br />
        #ACT<br />
        MISSION 0 492 246 //怪物集中点<br />
        PARAM1 492 //刷出坐标<br />
        PARAM2 246   //刷出坐标<br />
        PARAM3 1 //数量<br />
        PARAM4 1 //范围<br />
    MOBPLACE 恐之心魔</p></td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">150</td>
    <td width="500"><p>Race:150 RaceImg:17 <br />
      //此怪物2种攻击特效，近战 + 远程 ，间隔一个身位平砍，DC-DCMAX   为近战伤害，远程追击并攻击目标，MC-SC 为远程伤害！<br />
      <br />
      Race:150 RaceImg:18 <br />
      //此怪物2种攻击特效，远程 + 近战   ，远程追击并攻击目标， MC-SC 为远程伤害！近身间隔一个身位攻击，DC-DCMAX 为近战伤害！<br />
      <br />
      Race:150 RaceImg:19<br />
//此怪物2种攻击特效，近战 + 近战 ，间隔一个身位平砍，DC-DCMAX 为近战伤害，间隔一个身位平砍，MC-SC 为近战伤害！ <br />
<br />
      Race:150   RaceImg:20 //此怪物1种攻击特效，近战 + 爆炸 ， 间隔一个身位平砍，DC-DCMAX 为近战伤害，死亡有1/5爆炸，MC-SC 为爆炸伤害！ </p>
    <p>锋喙修罗：Race：150 RaceImg：17<br />
        七杀修罗：Race：150 RaceImg：19<br />
        破军修罗：Race：150   RaceImg：17<br />
        贪狼修罗：Race：150 RaceImg：17<br />
        雷霆修罗：Race：150   RaceImg：18<br />
    金刚修罗：Race：150 RaceImg：20</p></td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">200</td>
    <td width="500">隔一格就会攻击，然后移动到身边，主动攻击</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">201</td>
    <td width="500">主动近身攻击</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">202</td>
    <td width="500">蛇妖王 ，怪物数据库 Mc - Sc 为冰锥的伤害设置！</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">203</td>
    <td width="500">全屏攻击，有石头掉下效果，被攻击者有1秒左右的卡步----投石巨魔</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">204</td>
    <td width="500">尸霸 Race：204 Raceimg：14 Appr： 69 //老尸霸，无攻击特效，无出生效果， 攻击附带麻痹效果，可在引擎上设置；<br />
    新尸霸   Race：204 Raceimg：15 Appr：542 //新尸霸拥有2种攻击特效，近战和近身AOE伤害，且有出生特效，攻击附带麻痹效果，可在引擎上设置；</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">205</td>
    <td width="500"><p>道士宝宝强化骷髅、龙骨骷髅专属AI，可配合引擎面板，怪物设置进行相关参数设置！<br />
    <br />
    </p></td>
    <td width="500">强化骷髅:   race=205，raceimg=10，appr=117<br />
龙骨骷髅: race=205，raceimg=23，appr=207</td>
  </tr>
  <tr>
    <td style="text-align: center">206</td>
    <td width="500">近战带绿毒攻击，怪物数据库 Mc 为绿毒点数，SC 为绿毒时间！(用于鬼方火卒)</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">207</td>
    <td width="500">近身距离三吐火攻击 (地火兽骑将、教主坐骑) </td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">208</td>
    <td width="500">麻痹近身攻击，会移动，强--这个几率是100%的麻痹</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">209</td>
    <td width="500">追杀天玉公主怪物</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">210</td>
    <td width="500">固定不会移动，远程攻击--仙人掌</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">211</td>
    <td width="500">替身，此怪物是技能替身法符的怪物</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">212</td>
    <td width="500">图腾类怪物</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">213</td>
    <td width="500">啸天虎</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">214</td>
    <td width="500">俘虏”类型怪物不攻击，不反击，当超过CoolEye设定范围后，将停止走动</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">215</td>
    <td width="500">镖车专用AI <br />
      MP：镖车提示位置间隔时间，单位：秒<br />
      DC：为镖车攻击真实伤害，百分比掉血<br />
      MC：等级控制。小于MC等级的玩家攻击镖车会触发反弹功能<br />
    SC：反弹比列。设置50则表示玩家攻击镖车的伤害50%会减少自己的HP</td>
    <td width="500">&nbsp;</td>
  </tr>
  <tr>
    <td style="text-align: center">254</td>
    <td width="500"><p>心魔类型怪；<br />
      RaceImg代码：<br />
      255有烟雾; <br />
      254:   无烟雾、无尸体; <br />
    253: 有尸体、无烟雾(夺宝心魔) </p></td>
    <td width="500">&nbsp;</td>
  </tr>
</table>