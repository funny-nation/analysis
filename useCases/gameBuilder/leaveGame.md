## 步骤4 离开游戏
### 描述

玩家取消reaction退出游戏

### 角色

点击了reaction的用户

### 触发

当用户想离开游戏时

### 数据输入（来源）

取消reaction（点击reaction的用户）

### 数据输出（去向）

是否退出了游戏（私信用户）

### 路径

1. 户可以取消reaction“🟣”退出游戏
2. “bot”私信用户```您已退出游戏```
3. “bot”在原有embed里，撤回（删除）@user_name，https://github.com/funny-nation/embed-sand-box/blob/main/embed/dealer.py

### 扩展路径
