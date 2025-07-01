# FearMelts

## Overview
A connector for integrating ChatGPT capabilities into your applications or workflows. This project provides a simple interface to interact with OpenAI's ChatGPT API, making it easy to add conversational AI features to your software.

## Prerequisites
- [Node.js](https://nodejs.org/) (v14 or higher recommended)
- An OpenAI API key ([get one here](https://platform.openai.com/account/api-keys))

## Installation
1. **Clone the repository:**
   ```sh
   git clone https://github.com/FearMelts/FearMelts.git
   ```
2. **Navigate to the project directory:**
   ```sh
   cd FearMelts
   ```
3. **Install dependencies:**
   ```sh
   npm install
   ```

## Configuration
1. **Set your OpenAI API key.** You can do this by creating a `.env` file in the project root:
   ```env
   OPENAI_API_KEY=your_openai_api_key_here
   ```
   Or, you can pass the API key directly in your code (see below).

## Usage
Here is a basic example of how to use FearMelts in a Node.js project:

```js
const FearMelts = require('./FearMelts');

const connector = new FearMelts({
  apiKey: process.env.OPENAI_API_KEY, // or put your key directly here
});

connector.sendMessage('Hello, ChatGPT!').then(response => {
  console.log('ChatGPT says:', response);
}).catch(err => {
  console.error('Error:', err);
});
```

**Note:** Replace `process.env.OPENAI_API_KEY` with your actual API key if not using environment variables.

For more advanced usage and configuration, see the documentation or source code.

## Features
- Easy integration with ChatGPT
- Customizable settings
- Supports multiple platforms (Node.js, browser, etc.)
- Simple API for sending and receiving messages

## Contributing
Contributions are welcome! Please open issues or submit pull requests. Make sure to follow the code style and include tests for new features.

## License
MIT License. See `LICENSE` file for details.