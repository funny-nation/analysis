## 步骤1 创建游戏
### 描述

 用户需要自定义卡牌内容让bot发起组局邀请，由玩家自行进入游戏对局

### 角色

 服务器内任意用户

### 触发

 当用户想开始一局新的游戏时

### 数据输入（来源）

 包括游戏名称，卡牌名称和数量（用户给bot）

### 数据输出（去向）

 游戏名称，卡牌名称和游戏人数（bot给用户）

### 路径

1. 用户私信“bot”指令： ```创建游戏 狼人杀 狼 1 村民 3```其中狼人杀表示游戏名称，狼表示角色名称，3表示狼牌数量
2. "bot"检测该用户是否有重名的游戏
3. “bot”检测数字是不是大于0的正整数
4. “bot”在指定频道发布游戏发牌通知，https://github.com/funny-nation/embed-sand-box/blob/main/embed/dealer.py （还没改完）
5. “bot”在步骤#4.的消息结尾添加reaction“🟣” 
6. “bot”检测点击reaction的人数是否为游戏总人数
7. “bot”私信回复用户```已有足够的人，可以建立游戏```

### 扩展路径

 1. 如果数字不是大于0的正整数，“bot”私信发布者回复```牌的数量只能是正整数哦```
 2. 如果有重名的游戏，“bot”私信发布者回复```游戏名不可重复哦```
