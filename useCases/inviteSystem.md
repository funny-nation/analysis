### 描述

服务器内用户可以通过邀请其他玩家获取货币

### 角色

服务器内任意用户

### 触发

当用户的邀请链接被使用时

### 数据输入（来源）

其他用户点击邀请链接进入服务器

### 数据输出（去向）

创建链接的玩家收到货币

### 路径

1. “bot”检查用户是否创建了邀请链接（用户可以创建多个邀请链接）
2. "bot"检查一周前有多少用户使用了邀请链接（这周日检查上周日用的）
3. “bot”检查使用邀请链接的人是否还在dc（在1周了）
4. “bot”检查使用邀请链接的人是否在dc发送过文字消息
5. “bot”给创建链接的玩家定期发放奖金，每天发放一次，35货币/人

### 扩展路径

1. 如果玩家没有创建邀请链接，则无效
2. 如果玩家的链接一周前没有被使用，则无效
3. 如果玩家邀请的用户不在dc了，则无效
4. 如果玩家邀请的人没有发过文字信息，则无效
