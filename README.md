# node-getui
不知道为啥个推不把 SDK 放上来。无法用 npm 装。本仓库单纯做了一个方法整理，加速开发。

# 安装方法

```
npm install getui-node -S
```

# 使用方法（暂时只有一个向单人发推送的方法，后续看需要补充

```javascript
		var getui = require('getui-node').init(HOST, APPID, APPKEY, MASTERSECRET)
		
		getui.pushMessageToSingle(clientId, '内容测试',2, '测试通知', 0, null).then(function(data){
			console.log(data)
		}, function(err){
			console.error(err)
		})
```
