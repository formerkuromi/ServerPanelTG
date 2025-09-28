# Telegram bot for server management
A Telegram bot for managing a server and processes running on it.

## Features

### PM2 process management
- View PM2 process status
- Stop a PM2 process
- Restart a PM2 process
- Start a PM2 process

### Server commands
- Reboot the server
- Update server packages
- Update projects from GitHub

## Bot demo
Overview of bot features and setup instructions - [Watch on YouTube](https://youtu.be/Mu7h2maLMUc)  

## Deploying the bot to a server
Video guide on deploying a Telegram bot to a server - [Watch on YouTube](https://youtu.be/vPqAYdjkm4o)  

* Install Git and update system components
```bash
sudo apt update
sudo apt install git
```

* Clone the repository with the bot to the server:
```bash
git clone https://github.com/formerkuromi/ControlServerBot.git
```

* Go to the project folder:
```bash
cd ControlServerBot
```

* Install Node.js and npm package manager
```bash
sudo apt install nodejs
sudo apt install npm
```

* Update Node.js and npm, then restart the server
```bash
sudo npm install -g n
sudo n stable
```

* Install all dependencies
```bash
cd ControlServerBot
npm i
```

* Create a global variable file
```bash
nano .env
```

* Inside the `.env` file, create the following variables:
```bash
BOT_API_KEY=''
SERVER_HOST=''
SERVER_USERNAME=''
SERVER_PASSWORD=''
ADMIN_ID=''
PROJECT_PATHS='name1:path to project folder,name2:path to project folder'
```

* Install pm2 to run the bot
```bash
npm i pm2 -g
```

* Start the bot on the server
```bash
pm2 start index.js
```

## grammy js documentation

[grammy js documentation](https://grammy.dev/guide/)


## Author

- [@formerkuromi](https://github.com/formerkuromi)

© 2025 formerkuromi (Denys). All rights reserved.
