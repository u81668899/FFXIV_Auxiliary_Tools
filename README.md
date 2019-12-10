﻿# FFXIV_Auxiliary_Tools
**最终幻想14 5.0 暗影之逆焰 轮椅辅助工具**
    
    BUG反馈/交流群:868116069
## Hojoring-SPESPE时间轴 (中/日/英)
-  支持副本
    - 伊甸希望乐园：觉醒篇
    - 伊甸零式希望乐园：觉醒篇（测试版）
    - 无瑕灵君歼殛战
    - 缇坦妮雅歼殛战
#### 通用
- 死刑、AoE、月环、核爆等普通机制的TTS
#### 缇坦妮雅歼殛战
- 随机幻影符文是靠近还是远离。
#### 无瑕灵君歼殛战
- 断罪飞翔的机制效果
- 断罪之桩判定倒计时
####  伊甸零式希望乐园：觉醒篇 1 层
- 告知 **\[正/反\]三角攻击**    处理方法
- 告知 **\[正/反\]恶习与美德**  处理方法
- 奶妈传毒提醒
- 失乐园诱导报数
#### 伊甸零式希望乐园：觉醒篇 2 层
- 巨腕技能提升
- 以实际判定为准进行提示
#### 伊甸零式希望乐园：觉醒篇 3 层
- 俯冲攻击躲避位置
- 大海啸1直线点名提示
- 大海啸2根据不同BUFF的处理方法（amaya式，T参与44分摊）
#### 伊甸零式希望乐园：觉醒篇 4 层
- 二穿一倒计时
- 冲拳顺序
- 砸地板方位
- 岩盘崩落你要去的位置（根据子言视频攻略）
- 升降梯机制你要去的位置（根据子言视频攻略）
- 白流沙自己所要在的地板位置（战斗前需设置）（根据子言视频攻略）

### 删除TTS
- 临时删除
    - 编辑文件将位于上部的TTS部分注释/删除：例```<!-- 被注释的内容 -->```
    - 变量形式的TTS：例```var AoE_TTS = "大伤害AoE"```改为```var AoE_TTS = ""```
- 我永远都不需要触发器和TTS，别占我资源：
    - 把除了时间轴本体`<s>`标签以外的`<s>`与`<t>`标签与`Razor语句`都删掉。
### 自定义样式
- 背景  
    一个透明无颜色的配置是#00000000  
    第1-2位是背景的不透明度的16进制 如果你想要透明50%(127),则为"7F"  
    第3-4位是颜色的R值的16进制  5-6位是G值的16进制 7-8位是B值的16进制  
    所以先找到一个喜欢的颜色，再将他们三位RGB值分别转换为十六进制即可。
    例如你想要一个RGB(0,108,191)透明度为90%的蓝色背景，设置则应该填入：#E6006CBF  
    [在线进制转换网站](https://tool.oschina.net/hexconvert)

- 内部样式
    样式名|填充颜色|轮廓颜色 
    -|-|-|
    AoE|#FF9370DB|#FF000000
    分摊|#FF00B2ED|#FF000000
    死刑|#FFE93F00|#FF000000
    伤害|#FFEDCA00|#FF000000
---
## Hojoring-SST技能触发器
- 团辅监控 (中/日/英)
    - 背刺 鼓励 连环计 灵护 义结金兰 战斗连祷 巨龙视线 战斗之声 技巧闭幕 进攻探戈 占卜
---
## Triggernometry
- Actor Tick Timer 1.1 国服适用版
    - 需自行配置`Actor tick track visual`与`Initiate`的`Image aura Path`
- 大技能TTS (中/日/英)
    - 超火流星 行尸走肉 神圣领域 圣光幕帘 死斗 死而不僵 天赐祝福
---