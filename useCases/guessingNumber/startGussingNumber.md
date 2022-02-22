### 描述

服务器内用户可以猜数字玩儿，增加娱乐性

### 角色

服务器内任意用户

### 触发

当用户想玩儿猜数字时

### 数据输入（来源）

任意用户

### 数据输出（去向）

任意用户

### 路径

1. 用户在频道内输入```ghs 开局猜数字```，默认范围是0-100
2. "bot"回复https://github.com/funny-nation/embed-sand-box/blob/main/embed/guessNumber.py
3. 在步骤#2消息结尾添加reaction"🔢"
4. 用户点击reaction“🔢”加入组局，“bot”发送```user_name已加入对局```
5. "bot"在后台生成一个0-100范围内的随机数字

### 扩展路径

