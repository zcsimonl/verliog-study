# day2.2019.4.23
打卡
1. 画一下电路图：CMOS反相器、与非门、或非门、三态输出门、漏极开路门
  见DOC文件
2.解释一下vih,vil,vol,voh,vt,Iddq
Vil表示最大可靠输入低电平电压Vil(max);
vih表示最小可靠输入高电平电压Vih(min);//逻辑电路可靠工作的条件，输入高电平必须大于vih,输入低电平电压必须小于vil.
voh:输出最小合格高电平电压
vol:输出最大合格低电平电压
vt:mos管的闸值电压
Iddq:集成电路静止电流（integrated Circuit Quiescent current）器件不受外部因素影响下本身消耗电流。
3.CMOS反相器的速度与那些因素有关？什么是转换时间（transition time）和传播延迟（propagation delay）
  速度与负载电容，自载电容，连线电容，输出电阻有关
  提高电源电压，提高电源电压可以降低延时，即用功耗换取性能但超过一定程度后改善有限
  加大晶体管的尺寸（驱动能力），使晶体管的等效导通电阻（输出电阻）较小。但这同时加大自载电容和负载电容（下一级晶体管的输入电容）
  转换时间：电平的上时间和下降时间
  传播延迟：在输入信号变化到50%Vdd到输出信号变化到50%Vdd之间的时间。
4.反相器的功耗主要包括哪几部分？分别与那些因素有关？
   主要包括静态功耗和动态功耗，其中主要由动态功耗影响，动态功耗由两部分主城：开关电流和短路电流。 功耗主要频率和负载电容，电路电压有关
   p=C*V*Vf;
5.什么是latch-up效应
  cmos晶片中，在电源和地线之间由于寄生的PNP和NPN双极性BJT相互影响而产生的低阻抗通路。
6. 相同面积的cmos与非门和或非门哪个更快
  互补cmos电路中，与非门采用PMOS管并联，NMOS管串联，或非门才哦哦那个PMOS管串联，NMOS管并联，PMOS采用空穴导电，NMOS采用电子导电，PMOS的载流子的迁移率比NMOS的迁移率小。同样尺寸条件下，PMOS的充电时间要大于NMOS的充电时间，因此与非门速度较快。
  
