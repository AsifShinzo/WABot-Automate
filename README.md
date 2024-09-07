## WhatsApp Bot - Simplify and Automate Your WhatsApp Experience

This project offers a simple yet powerful WhatsApp bot built in JavaScript, designed to streamline your daily tasks. Using the **@whiskeysockets/baileys** library, it leverages WebSocket connections for enhanced performance without relying on Puppeteer or Chromium.

### Key Features

- **Automate repetitive tasks** to enhance your WhatsApp experience.
- Built using the **Baileys library**, a feature-rich solution that directly operates on WebSockets.
  
### Prerequisites

Ensure you have the following installed on your system:

- **Node.js LTS (v20 or later)** for executing JavaScript code
- **FFmpeg** to process media files
- **Git** for managing the project repository
- **PM2** (optional) for efficient production deployment

### Setup Guide

1. **Clone the Repository:**

   Begin by cloning the project from GitHub:

   ```bash
   git clone https://github.com/AsifShinzo/WABot-Automate
   ```

2. **Navigate to the Project Directory:**

   Move into the project folder:

   ```bash
   cd WABot-Automate
   ```

3. **Update Configuration:**

   Open the `src/config.json` file and update it with your owner numbers:

   ```json
   {
     "ownerNumbers": ["YOUR_NUMBER", "ANOTHER_NUMBER"]
   }
   ```

   Replace `"YOUR_NUMBER"` and `"ANOTHER_NUMBER"` with the actual WhatsApp numbers that should have admin privileges.

### Running the Bot

You have two options to run the bot: directly using Node.js or using PM2 for a more robust production environment.

#### 1. Run with Node.js:

   ```bash
   export asif && node src/index.js BOT_NUMBER
   ```

   Replace `BOT_NUMBER` with the actual bot's phone number.

#### 2. Run with PM2 (Recommended for Production):

   ```bash
   pm2 start ecosystem.config.js -- BOT_NUMBER
   ```

   This method ensures the bot stays online, even after closing your terminal.

### Key Files

- **src/config.json**: Contains the configuration details like owner numbers and other customizable settings.

### License

This project is licensed under the MIT License. For more details, see the [LICENSE](LICENSE) file.
