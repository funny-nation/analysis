### 描述

用户在频道看到红包，并且过来抢

### 角色

任何用户

### 触发

当用户看到有人发红包时

### 数据输入（来源）

1. 是否抢（用户）

### 数据输出（去向）

1. 是否成功（用户）
2. 抢到了多少钱（用户）

### 路径

1. “用户”点击已经添加的“💰”Reaction。
2. “Bot”检查后台的红包数量。
3. “Bot”改变后台红包，并且获得所抢到的金额。
4. “Bot”把抢到的金额加到“用户”的余额中。
5. “Bot”在该频道发消息```user_name，恭喜你抢到了xx元```，其中user_name代表用户名。


### 扩展路径

2. 
	1. 如果后台红包已经抢完了
		1.  “Bot”回复```user_name，你来晚了，红包被抢完了```，其中user_name代表用户名。
		2.  结束
	

