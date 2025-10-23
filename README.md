# Aurevix Telegram Bot

A friendly, witty AI chatbot for Telegram powered by DeepSeek R1 through OpenRouter. Aurevix provides natural, human-like conversations right in your Telegram chats.

## 🚀 Try It Now!

**Live Bot**: [@aurevix_bot](https://t.me/aurevix_bot)

Chat with Aurevix directly on Telegram - no setup required!

## Features

- 🤖 AI-powered conversations using DeepSeek R1 model
- 💬 Natural, friendly, and engaging responses
- ⚡ Real-time message handling
- 🎯 Simple and lightweight implementation
- 🔄 Continuous polling for instant responses

## Prerequisites

- Python 3.7 or higher
- A Telegram Bot Token (from [@BotFather](https://t.me/botfather))
- An OpenRouter API Key (from [OpenRouter.ai](https://openrouter.ai))

## Installation

1. **Clone the repository**
   ```bash
   git clone <your-repo-url>
   cd <your-repo-name>
   ```

2. **Install required dependencies**
   ```bash
   pip install requests
   ```

3. **Configure the bot**
   
   Open `bot.py` and update the following configuration variables:
   ```python
   BOT_TOKEN = "your-telegram-bot-token"
   OPENROUTER_API_KEY = "your-openrouter-api-key"
   YOUR_SITE_URL = "your-site-url"  # Optional
   YOUR_SITE_NAME = "your-site-name"  # Optional
   ```

## Getting Your API Keys

### Telegram Bot Token
1. Open Telegram and search for [@BotFather](https://t.me/botfather)
2. Send `/newbot` and follow the instructions
3. Copy the bot token provided

### OpenRouter API Key
1. Visit [OpenRouter.ai](https://openrouter.ai)
2. Sign up or log in
3. Navigate to the API Keys section
4. Generate a new API key

## Usage

1. **Start the bot**
   ```bash
   python bot.py
   ```

2. **Chat with your bot**
   - Open Telegram and search for your bot
   - Send `/start` to begin
   - Start chatting!

## Commands

- `/start` - Initialize the bot and get a welcome message
- Any text message - Get an AI-powered response from Aurevix

## How It Works

1. The bot continuously polls the Telegram API for new messages
2. When a message is received, it's sent to OpenRouter's API
3. DeepSeek R1 model processes the message with Aurevix's personality
4. The response is sent back to the user via Telegram

## Configuration Options

You can customize the bot by modifying these settings in `bot.py`:

- `MODEL_NAME` - Change the AI model (default: deepseek/deepseek-r1-0528-qwen3-8b:free)
- System prompt in `ask_openrouter()` - Adjust Aurevix's personality
- Polling interval in `main()` - Change response frequency (default: 1 second)

## Troubleshooting

**Bot not responding?**
- Check your internet connection
- Verify your API keys are correct
- Ensure the bot token is valid
- Check the console for error messages

**API errors?**
- Verify your OpenRouter API key has credits
- Check if the model name is correct
- Review OpenRouter's API status

## Security Notes

⚠️ **Important**: Never commit your API keys to version control!

- Remove sensitive data before pushing to GitHub
- Use environment variables for production deployments
- Consider using a `.env` file with `python-dotenv`

## Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new features
- Submit pull requests

## License

This project is open source and available under the MIT License.

## Support

For issues and questions:
- Open an issue on GitHub
- Check [OpenRouter documentation](https://openrouter.ai/docs)
- Review [Telegram Bot API docs](https://core.telegram.org/bots/api)

---

Made with ❤️ by Sahin Enam