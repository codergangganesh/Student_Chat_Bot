# AI Chat Bot

An advanced chatbot application powered by Google's Gemini AI model that allows users to have intelligent conversations and even analyze images.

## Table of Contents
- [AI Chat Bot](#ai-chat-bot)
  - [Table of Contents](#table-of-contents)
  - [Features](#features)
  - [Technologies Used](#technologies-used)
  - [Setup Instructions](#setup-instructions)
  - [How It Works](#how-it-works)
  - [API Integration](#api-integration)
  - [File Structure](#file-structure)
  - [Usage](#usage)
  - [Responsive Design](#responsive-design)
  - [License](#license)
  - [Author](#author)

## Features

- **AI-Powered Conversations**: Chat with an AI assistant powered by Google's Gemini model
- **Image Analysis**: Upload images and ask questions about them
- **Real-time Responses**: Get instant replies from the AI
- **Modern UI**: Clean and intuitive chat interface
- **Loading Indicators**: Visual feedback during AI processing
- **Responsive Design**: Works on both desktop and mobile devices
- **Image Support**: Send images along with text messages

## Technologies Used

- HTML5
- CSS3
- JavaScript (ES6+)
- Google Gemini AI API
- Fetch API for HTTP requests
- Base64 encoding for image processing

## Setup Instructions

1. Clone or download this repository
2. Open `index.html` in your web browser
3. Start chatting with the AI assistant!

**Note**: The application uses a Google API key that's already included in the code. For production use, you should generate your own API key from the Google AI Studio.

## How It Works

1. **User Input**: Users type messages in the input field at the bottom of the chat interface
2. **Message Processing**: When a message is sent, it's displayed in a user chat bubble on the right side
3. **AI Request**: The application sends the user's message to Google's Gemini AI API
4. **Response Handling**: The AI's response is received and displayed in an AI chat bubble on the left side
5. **Image Support**: Users can upload images which are converted to base64 and sent with the message to the AI for analysis

## API Integration

The chatbot uses Google's Gemini Flash model via the following endpoint:
```
https://generativelanguage.googleapis.com/v1beta/models/gemini-1.5-flash:generateContent
```

The API key is included in the JavaScript code. For production deployment, it's recommended to:
1. Generate your own API key from [Google AI Studio](https://aistudio.google.com/)
2. Store it securely (e.g., in environment variables)
3. Update the `Api_Url` variable in [script.js](script.js)

## File Structure

```
.
├── index.html          # Main HTML structure
├── style.css           # Styling and layout
├── script.js           # JavaScript functionality
├── ai.png              # AI avatar image
├── user.png            # User avatar image
├── background.jpg      # Chat background image
├── chatbackground.jpg  # Input area background
├── img.svg             # Image upload icon
├── submit.svg          # Submit button icon
└── loading.webp        # Loading animation
```

## Usage

1. Type your message in the input field at the bottom
2. Press Enter or click the submit button to send
3. View the AI's response in the chat area
4. To analyze an image:
   - Click the image button
   - Select an image from your device
   - Send your message with the image
5. The AI will process both text and image content

## Responsive Design

The chat interface is fully responsive and adapts to different screen sizes:
- On mobile devices (screens less than 600px wide):
  - Chat bubbles take up more screen width
  - Layout adjusts for better mobile experience

## License

This project is open source and available under the [MIT License](LICENSE).

## Author

**Mannam Ganesh Babu** - CEO

---
*This README was automatically generated for the AI Chat Bot project*
