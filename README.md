# wordbook

做这个项目的目的是为了自己背GRE单词，如果能给你带来一点帮助的话，我也是很开心的

version: 1.0

目前只能背GRE单词,未来会支持单词导入的 hhh

## 功能

1. 本程序使用python开发,兼容了在window的cmd中运行
2. 可以设置每日背诵计划
3. 使用记忆曲线自动筛选每日复习单词
4. 自动获取单词发音

## 使用方法

note: 由于这个程序只在window上测试过，所以不确定对linux或mac的兼容性

note: 需要提前配置程序的依赖环境 详细配置在requirement.txt内

启动方式：



Step 1:

在cmd中

~~~cmd
python program.py
~~~

![1](https://github.com/wgr5600133/wordbook/blob/main/readme_image/1.png)

由于cmd中可能会出现中文字体编码问题,如果你在第一步看不到中文,请选择n



Step 2:

如果你是第一次试图用这个程序,则它会询问你的单词计划

![3](https://github.com/wgr5600133/wordbook/blob/main/readme_image/3.png)

如果你不是第一次使用这个程序,则它读取你之前设置的计划并开始运行

![2](https://github.com/wgr5600133/wordbook/blob/main/readme_image/2.png)



Step3：

在这一步你可以选择更改你之前的计划,或者开始愉快的背单词啦~

## 遗忘曲线

遗忘次数 VS 遗忘几率

算法: p = e^(1/(t*s)*100) 

t为从开始日期到当前日期的天数差值

s为遗忘权重 算法为 log(1/x) x为背诵次数

Day 1:

![day1](https://github.com/wgr5600133/wordbook/blob/main/figures/day1.png)

Day 2:

![day2](https://github.com/wgr5600133/wordbook/blob/main/figures/day2.png)

Day 4:

![day4](https://github.com/wgr5600133/wordbook/blob/main/figures/day4.png)

Day 7:

![day7](https://github.com/wgr5600133/wordbook/blob/main/figures/day7.png)

Day 15:

![day15](https://github.com/wgr5600133/wordbook/blob/main/figures/day15.png)



## 联系方式

如果在使用过程中发现任何问题和bug 欢迎联系我 GUW18@pitt.edu
