### 描述

玩家点击reaction加入游戏

### 角色

服务期内所有用户

### 触发

当用户想加入游戏抽牌时

### 数据输入（来源）

点击reaction

### 数据输出（去向）

是否加入了游戏（私信用户）

### 路径

1. 服务期内用户可以点击reaction“🟣”加入游戏
2. “bot”检测是否人已经满了
3. “bot”私信用户```您已加入游戏，请等待发牌```
4. “bot”在原有embed里，添加@user_name，https://github.com/funny-nation/embed-sand-box/blob/main/embed/dealer.py

### 扩展路径

2. 如果人已经满了，“bot”私信回复```人已经满了，下局再来吧```
