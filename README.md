# Description
	
Telegram pubsub bot that notifies you whenever any of your deposits may be liquidated


## Deploy
This project uses javascript, nodejs and typescript standards.
Copy files from json_dir directory to home directory.

Use node package manager (npm) to deploy the project:
```
npm install # Install dependencies
npm run patch-tbtc # Transpile tbtc package
npm run build # Compile typescript code & apply transpilations
npm run lint # Lint & format code
npm start # Start the bot

```
## Configuration
The configuration (tsconfig.json) describes typescript to javascript conversion forms according to es5 specification
```json
{
  "compilerOptions": {
    "target": "es5",
    "strict": true,  
    "esModuleInterop": true,
    "allowJs":true,
    "skipLibCheck": false, 
    "outDir": "build",
    "forceConsistentCasingInFileNames": true,
    "noUnusedLocals": true,
    "declaration": true,
    "noUnusedParameters": true
  },
  "exclude": ["node_modules", "build"]
}
```

## How to use this bot

1. Start a chat with t.me/tbtc_liquidations_bot on Telegram.
2. The bot will respond with further instructions on how to subscribe to undersupply alerts..

## Hosting your own
To host your own bot (improved privacy, no need to trust me, increased resilience to attacks...) you should follow these steps:
1. Create a Telegram bot through [@BotFather](t.me/BotFather)
2. Deploy the code for this project on Heroku
3. When asked for a token on heroku app creation screen input the token received on step 1, it should look something like `1066870955:AAGgA7X3b-dHAAWvK_stTpboqCh0pWGfn20`
4. Allow a few mins for heroku to spin up a server and your bot should be available at the handle that you chose on step 1, just start a chat and he'll reply with the usage instructions

## Useful links  
https://core.telegram.org/bots#creating-a-new-bot  
https://heroku.com/deploy

### Disclaimer:

This software is provided "as is", without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose and noninfringement. In no event shall the authors or copyright holders be liable for any claim, damages or other liability, whether in an action of contract, tort or otherwise, arising from, out of or in connection with the software or the use or other dealings in the software.
