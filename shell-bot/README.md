## condition
服务器需要预装环境：nodejs pm2

## Obtain your Chat id
在浏览器打开：https://api.telegram.org/bot[API Token]/getUpdates //将[API Token]替换成自己的API token
然后给你的机器人发送消息，就能再这个地址的页面获取到你的chat id
## Config
获取你的Telegram的ID和机器人的Token写入config.js配置文件
```javascript
module.exports = {
    config:function(){
        return (
            {
                adminUsers:[ADMIN_ID], //你的telegram ID应该是数字
                botToken: 'YOUR_BOT_TOEKN', // 机器人Token

            }
        );
    }
};
```
## Run
```
npm start
```
or 
```
node index.js
```
## pm2
```
pm2 start pm2.json
```

That is it!
