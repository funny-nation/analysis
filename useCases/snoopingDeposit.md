### 描述

用户可以偷看其他用户的账户余额

### 角色

服务器内任意用户

### 触发

当有人想偷看其他用户的余额时

### 数据输入（来源）

服务器内用户

### 数据输出（去向）

服务器内用户

### 路径

1. 用户在服务器内输入指令```ghs 偷看 @user_name```，其中@user_name是被偷看的用户id
2. “Bot”私信输入指令的用户“指定用户”的账户余额信息：```偷偷告诉你，user_name还有1000元！```,其中1000指指定用户的账户余额
3. 用户每使用一次此功能，将转账200货币给被偷看余额的人

### 扩展路径

1. 输入指令的用户余额不足200时，bot私信```穷逼，别看了，肯定比你有钱！```

