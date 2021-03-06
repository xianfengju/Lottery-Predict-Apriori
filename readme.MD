# 福彩双色球预测 Apriori算法


## 1. 需求描述
给定2013,2014,2015,2016的福彩双色球数据.
输出:给出前区(红球)数据(6个号码)的预测至少一注(一条比如 2 5 13 14 26 33),后区(蓝球)那个号码不处理。
设计一种预测算法，并实现。

## 2. 预测方法
利用Apriori算法，得出频繁五项集和频繁一项集的集合，将频繁一项集中支持度最高的球号与频繁五项集减去带有支持度最高的球号的子集进行拼接，并规定将支持度最高的频繁一项集放在每个事务的最前面。

## 3. 运行环境
python3.4+

## 4. 运行结果截图
![apriori][img1]

## 5. 预测结果
- 14，11，16，2，26，4
- 14，10，11，12，15，32
- 14，10，15，20，23，31
- 14，1，10，11，13，32
- 14，13，16，22，25，27
- 14，13，18，5，6，7
- 14，17，22，3，32，33
- 14，10，15，22，29，8
- 14，10，12，2，30，4
- 14，1，2，22，28，30
- 14，13，2，20，22，3
- 14，13，19，28，5，6
- 14，18，22，32，33，6

[img1]: https://raw.githubusercontent.com/HScarb/Lottery-Predict-Apriori/master/apriori.png