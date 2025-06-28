# AIChatBot: Full-Stack AI Chatbot with Local and Cloud LLMs

![AIChatBot](https://img.shields.io/badge/Download%20Releases-blue?style=for-the-badge&logo=github&link=https://github.com/Zabuzqdde/AIChatBot/releases)

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [API Documentation](#api-documentation)
- [Contributing](#contributing)
- [License](#license)

## Overview

AIChatBot is a full-stack AI chatbot that utilizes both local and cloud large language models (LLMs). This project combines a robust .NET 9 API with an Angular 20 user interface, allowing users to run models like PHI-3, Mistral, Gemma, and Llama3 either locally using Ollama or online via OpenRouter. The flexibility of this setup makes it easy to deploy and test various AI models in real-time.

## Features

- **Local and Cloud Models**: Run models locally with Ollama or access cloud models through OpenRouter.
- **User-Friendly Interface**: Built with Angular 20 for a seamless user experience.
- **Multiple Model Support**: Easily switch between different AI models like PHI-3, Mistral, Gemma, and Llama3.
- **Responsive Design**: Works on various devices, ensuring accessibility for all users.
- **Real-Time Interaction**: Engage with the chatbot in real-time for instant responses.
- **Extensive API**: A well-documented API for easy integration and customization.

## Technologies Used

- **Frontend**: Angular 20
- **Backend**: .NET 9 API
- **Local LLMs**: Ollama
- **Cloud LLMs**: OpenRouter
- **Operating System**: Windows Subsystem for Linux (WSL) on Ubuntu

## Installation

To get started with AIChatBot, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Zabuzqdde/AIChatBot.git
   cd AIChatBot
   ```

2. **Install Dependencies**:
   For the backend:
   ```bash
   cd backend
   dotnet restore
   ```

   For the frontend:
   ```bash
   cd frontend
   npm install
   ```

3. **Run the Application**:
   Start the backend server:
   ```bash
   dotnet run
   ```

   Then, start the frontend server:
   ```bash
   ng serve
   ```

4. **Access the Application**:
   Open your browser and navigate to `http://localhost:4200`.

5. **Download and Execute Releases**:
   For the latest releases, visit [Download Releases](https://github.com/Zabuzqdde/AIChatBot/releases) to download the necessary files.

## Usage

Once the application is running, you can interact with the chatbot through the Angular interface. Simply type your queries in the chat window, and the AI will respond in real-time. You can also switch between local and cloud models through the settings menu.

### Example Interaction

1. User: "What is the weather like today?"
2. Chatbot: "Today, you can expect sunny skies with a high of 75°F."

### Switching Models

To switch models, navigate to the settings panel and select your preferred model from the dropdown menu. This allows you to test different responses based on the model you choose.

## API Documentation

The API provides various endpoints to interact with the chatbot. Below are some key endpoints:

### GET /api/chat

- **Description**: Send a message to the chatbot and receive a response.
- **Parameters**:
  - `message`: The user's input message.

### POST /api/models

- **Description**: Get a list of available models.
- **Response**:
  - A JSON array of model names.

### Example Request

```bash
curl -X GET "http://localhost:5000/api/chat?message=Hello"
```

### Example Response

```json
{
  "response": "Hello! How can I assist you today?"
}
```

## Contributing

Contributions are welcome! If you would like to contribute to AIChatBot, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Make your changes and commit them (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a pull request.

Please ensure your code adheres to the existing coding style and includes appropriate tests.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

For more information, updates, and releases, visit [Download Releases](https://github.com/Zabuzqdde/AIChatBot/releases).