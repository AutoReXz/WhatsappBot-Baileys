# WhatsApp Bot using Baileys Library

A modular WhatsApp bot created with the WhiskeySockets/Baileys library.

## Installation

1. Clone this repository:
```
git clone <repository-url>
cd baileysss
```

2. Install dependencies:
```
npm install
```

3. Run the bot:
```
npm start
```

4. Scan the QR code displayed in the terminal with your WhatsApp app.

## Available Commands

All commands start with the `!` prefix. Current available commands:
- `!ping` - Check if bot is online
- `!echo [text]` - Repeat the text you send
- `!help` - Display all available commands

## Adding New Commands

To add a new command, simply create a new JavaScript file in the `commands` folder with the following structure:

```javascript
module.exports = {
    name: 'commandname',
    description: 'Description of what the command does',
    execute: async (sock, message, args, context) => {
        // Your command logic here
        // Use sock.sendMessage() to respond
    }
};
```

The commands will be automatically loaded - no restart needed!

## Logs

Logs are saved in the `logs` directory:
- `app.log` - Contains all application logs
- `error.log` - Contains only error logs

## Customization

You can customize the bot by:
1. Adding new commands to the `commands` folder
2. Modifying the message handler in `messageHandler.js`
3. Adjusting logging settings in `logger.js`
#   W h a t s a p p B o t - B a i l e y s  
 