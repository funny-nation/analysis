### 描述

抽奖发布者开奖

### 角色

抽奖发布者

### 触发

当抽奖发布者想要开奖

### 数据输入（来源）

抽奖活动发布者点击抽奖活动reaction“🟩”

### 数据输出（去向）

抽奖发布者昵称
中奖名单
奖品信息

### 路径

1. “bot”检查是否有足够人数参与抽奖
2. 抽奖活动发布者点击抽奖活动reaction“🟩”，“bot”在点击反应的用户中随机抽取相应数量的用户，发布获奖信息https://github.com/funny-nation/embed-sand-box/blob/main/embed/openLottery.py
```
恭喜 
@user_name
@user_name
@user_name
@user_name
@user_name
获得由@user_name送出的比心！
记得及时去兑奖哦！
```
3. 开奖后自动关闭抽奖活动
4. 只有抽奖活动发布者可以开奖或关闭抽奖
5. 开奖后购买抽奖券的货币计入发布者账户内

### 扩展路径

2. 参与抽奖人数不够的时候，活动发布者点击reaction“🟩”，“bot”回复```人数好像不够，等一下吧！```
