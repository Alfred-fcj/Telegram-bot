## condition
服务器需要预装环境：nodejs pm2

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
