# HUCM-2018蓝桥杯第1场选拔赛

## A. 计算两点间的距离

**Problem Description**    

输入两点坐标（X1,Y1）,（X2,Y2）,计算并输出两点间的距离。

**Input**

输入数据有多组，每组占一行，由4个实数组成，分别表示x1,y1,x2,y2,数据之间用空格隔开。
 

**Output**

对于每组输入数据，输出一行，结果保留两位小数。
 

**Sample Input**

    0 0 0 1
    0 1 1 0

 

**Sample Output**

    1.00
    1.41

## B. 小学生的游戏

**Problem Description**

某天，无聊的小斌叫上几个同学玩游戏，其中有比较笨的小兴，比较傻的小雪，可爱的小霞和自以为是的小楠。他们去找聪明的小明去给他们当裁判。判定谁取得游戏胜利。

而这个游戏是由小斌想个1到10000000的数字让大家猜，看谁先猜中。为了防止小斌作弊，小明记录下了游戏的整个过程。你的任务是判断小斌是否有作弊。

**Input**

输入数据包括多盘游戏。一次猜数包含两行，第一行是一个数字n(1<=n<=10000000)，表示所猜数字。第二行是小斌的回答为"too high","too low","right on"三种答案之一。每盘游戏结束于"right on"。当n=0的时候，整个游戏结束。

**Output**

对于每盘游戏，若小斌确有撒谎，请输出一行"The guy is dishonest",否则请输出"The guy may be honest"。

**Sample Input**

    10
    too high
    3
    too low
    4
    too high
    2
    right on
    5
    too low
    7
    too high
    6
    right on
    0

**Sample Output**

    The guy is dishonest
    The guy may be honest

## C. 石油管道

**Problem Description**

Oaiei居住在A城市，并且是这个城市建设的总设计师。最近有个问题一直困恼着他。A城市里有三个大型工厂，每个大型工厂每天都需要消耗大量的石油，现在城市里要建设一个石油中转站，从石油中转站到三个大型工厂都需要铺设石油管道。现在你的问题来了，应该如何建设这个石油中转站，使得石油中转站到三个大型工厂所需要铺设的石油管道线路最短，你能够帮助他吗？

设石油中转站B的坐标为(X,Y)，三个大型工厂的坐标分别为C(X1,Y1)，D(X2,Y2)，E(X3,Y3)，所输要铺设的石油管道线路总长为distance(B,C)+distance(B,D)+distance(B,E)，其中distance(A,B)表示A,B两点之间的欧几里德距离。

**Input**

第一行为一个整数C(1<=C<=200)，表示测试数据的组数。
以下C行，每行6个整数，分别表示C、D、E点 (X,Y)的坐标。注意：B点的选址可以与C、D、E点相重合。

**Output**

对于每个输入数据，输出一行两个数M1,M2，中间用一个空格分隔开。M1，M2分别四舍五入到小数点后两位，表示石油中转站的坐标。

**Sample Input**

    1
    0.00 0.00 1.00 0.00 0.00 1.00

**Sample Output**

    0.21 0.21

## D. 又见LKity

**Problem Description**

嗨！大家好，在TempleRun中大家都认识我了吧。我是又笨又穷的猫猫LKity。很高兴这次又与各位FZU的ACMer见面了。最近见到FZU的各位ACMer都在刻苦地集训，整天在日光浴中闲得发慌的我压力山大呀！于是，我准备为诸位编写一款小工具——LKity牌文本替换（众怒，：敢不敢更土点！）。这个小工具可以帮助诸位替换代码中的变量等功能，真心是一款编程，刷题必备的神器。其功能如下：

将给定的字符序列中所有包含给定的子串替换成另外一个给定的字符串。为了让其功能更加强大，替换过程中，将忽略大小写。并且不进行递归替换操作。

不过，作为笨笨的猫猫，我是心有余而力不足呀！希望诸位ACMer能帮我实现哈。（众FZU的ACMer：”……”）；

**Input**

输入包含多组数据。 输入为标准输入，输入包含3行。 第一行为需要查找的字符串S1。S1仅由大写或者小写字母组成，且其长度在区间[1，,100]内。 第二行为要替换的字符串S2。S2由[32,125]的字符组成，且其长度在区间[1,100]内。 第三行为原始字符串S，S由[32,125]的字符组成。且其长度在区间[1,50,000]内。

**Output**

对于每组数据，请输出替换后的字符串。

**Sample Input**

    abc
    bc ab
    aaa aaabca 333Abcc##

**Sample Output**

    aaa aabc aba 333bc abc##

## E. 数字的孔数

**Problem Description**

S得到一个数，他想知道这个数每一位上的数字的孔数之和。1,2,3,5,7这几个数字是没有孔的，0,4,6,9都有一个孔，8有两个孔。

**Input**

输入数据的第一行为一个数T表示数据组数。接下来T行，每行输入一个正整数n(1<=n<=1000)，表示要求数字孔数之和的数。n不会有前导0。

**Output**

对于每组数据输出一行一个整数，表示该数的每一位上的数字的孔数之和。

**Sample Input**

    2
    42
    669

**Sample Output**

    1
    3


## F. 简单的等式

**Problem Description**

现在有一个等式如下：x^2+s(x,m)x-n=0。其中s(x,m)表示把x写成m进制时，每个位数相加的和。现在，在给定n，m的情况下，求出满足等式的最小的正整数x。如果不存在，请输出-1。

**Input**

有T组测试数据。以下有T(T<=100)行，每行代表一组测试数据。每个测试数据有n（1<=n<=10^18），m(2<=m<=16)。

**Output**

输出T行，有1个数字，满足等式的最小的正整数x。如果不存在，请输出-1。

**Sample Input**

    4
    4 10
    110 10
    15 2
    432 13

**Sample Output**

    -1
    10
    3
    18

## G. 最长子串

**Problem Description**

问题很简单，给你一个字符串s，问s的子串中不包含s1,s2...sn的最长串有多长。

**Input**

输入包含多组数据。第一行为字符串s,字符串s的长度1到10^6次方，第二行是字符串s不能包含的子串个数n,n<=1000。接下来n行字符串,长度不大于100。

字符串由小写的英文字符组成。

**Output**

最长子串的长度

**Sample Input**

    lgcstraightlalongahisnstreet
    5
    str
    long
    tree
    biginteger
    ellipse

**Sample Output**

    12

## H. 分解素因子

**Problem Description**

假设x是一个正整数，它的值不超过65535(即`1<x<=65535`)，请编写一个程序，将x分解为若干个素数的乘积。

**Input**

输入的第一行含一个正整数k (1<=k<=10)，表示测试例的个数，后面紧接着k行，每行对应一个测试例，包含一个正整数x。

**Output**

每个测试例对应一行输出，输出x的素数乘积表示式，式中的素数从小到大排列，两个素数之间用“*”表示乘法。

**Sample Input**

    2
    11
    9828

**Sample Output**

    11
    2*2*3*3*3*7*13

## I. 穿越沙漠

**Problem Description**

一辆吉普车来到x公里宽的沙漠边沿A点，吉普车的耗油量为1升/公里，总装油量为500升。通常，吉普车必须用自身油箱中的油在沙漠中设置若干个临时储油点，才能穿越沙漠的。假设在沙漠边沿A点有充足的汽油可供使用，那么吉普车从A点穿过这片沙漠到达终点B，至少要耗多少升油。请编写一个程序，计算最少的耗油量（精确到小数点后3位）。

- （1）假设吉普车在沙漠中行进时不发生故障；
- （2）吉普车在沙漠边沿A点到终点B的直线距离为x≧500公里(即沙漠宽度)；

**Input**

输入的第一行含一个正整数k (1<=k<=6)，表示测试例的个数。后面紧接着k行，每行对应一个测试例，包含一个正整数x，表示从A点到B点的距离（1<=x<=2000）。

**Output**

每个测试例对应一行输出，包含一个数，表示最少的油耗量。

**Sample Input**

    2
    500
    1000

**Sample Output**

    500.000
    3836.497


## J. 神庙逃亡

**Problem Description**

话说最近穷猫猫LKity意外得到了一部ANDROID手机，于是，LKity兴奋地为自己的新机子安装了神往已久的游戏——神庙逃亡（Temple Run）。可惜，LKity不仅仅是一只穷猫猫，更是一只笨猫猫。每次她玩这款游戏的时候，都被群鄙视了。例如下图所示情形：

逃亡路途中，在Merida公主正前方S米出现了一堵火墙。火墙高度为H米。LKity控制着Merida公主以垂直方向上为Vy米/秒的速度试图跨越前方的火墙。已知现在Merida公主奔跑的速度（即水平速度）为Vx米/秒。你猜猜，笨笨的LKity能顺利控制Merida公主通过此障碍吗？【注：为了简便，在TempleRun的世界中，重力加速度恒为10m*s^-2】

**Input**

输入为标准输入，输入数据第一行为一个正整数T(1<=T<=100)表示接下来有T组测试数据 接下来为T行，每行一组数据，包括4个正整数S，H。Vx，Vy用空格隔开。其中，所有整数都在区间【1，1,000,000】内。数据保证S为Vx的倍数。

**Output**

对于每组数据，请输出一行，如果Merida公主能顺利通过前方火墙则输出“good done!”，否则输出“poor Merida!”。

**Sample Input**

    2
    100 1 1 1
    10 1 10 100

**Sample Output**

    poor Merida!
    good done!


-----


