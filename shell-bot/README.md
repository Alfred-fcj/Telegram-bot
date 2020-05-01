## condition
服务器需要预装环境：nodejs pm2

## Config
Follow [Telegram instructions](https://telegram.org/blog/bot-revolution) to create a bot
Then put your telegram user ID and bot token in `config.js`:
```javascript
module.exports = {
    config:function(){
        return (
            {
                adminUsers:[ADMIN_ID], //admin users' telegram id, should be numbers
                botToken: 'YOUR_BOT_TOEKN', // bot token

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
