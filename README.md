# VAPI AI Voice Assistant Demo

This project demonstrates how to integrate the VAPI AI voice and chat assistants into a React web application.

## Features

- Voice AI assistant with real-time conversation capabilities
- Text chat interface for alternate interaction
- Clean, modern UI with responsive design
- Easy configuration through environment variables

## Prerequisites

Before you begin, ensure you have:

1. A VAPI AI account (sign up at [https://vapi.ai](https://vapi.ai))
2. An assistant created in the VAPI AI dashboard
3. Your VAPI API key from the dashboard
4. Node.js and npm installed on your system

## Dependencies

This project uses the following key dependencies:

### Core Framework
- React 18.2.0
- React DOM 18.2.0
- TypeScript 4.9.5
- React Scripts 5.0.1

### VAPI AI Integration
- @vapi-ai/web 2.2.4 - Official VAPI AI SDK for web integration

### Utilities
- axios 1.6.2 - HTTP client for API requests
- uuid 9.0.1 - For generating unique IDs
- dotenv 16.3.1 - For environment variable management
- express 4.18.2 - For potential server-side functionality
- cors 2.8.5 - For handling CORS in API requests

### Type Definitions
- @types/react 18.2.0
- @types/react-dom 18.2.0
- @types/uuid 9.0.7
- @types/jest 27.5.2
- @types/node 16.18.126

## Setup Instructions

1. Clone this repository:
   ```
   git clone <repository-url>
   cd vapi-ai-assistant
   ```

2. Install dependencies:
   ```
   npm install
   ```

3. Configure your VAPI AI credentials:
   - Edit the `.env` file
   - Replace the placeholder values with your actual VAPI AI credentials
   ```
   REACT_APP_VAPI_API_KEY=your_actual_api_key
   REACT_APP_VAPI_ASSISTANT_ID=your_actual_assistant_id
   ```

4. Start the development server:
   ```
   npm start
   ```

5. Open your browser and navigate to `http://localhost:3000`

## Project Structure

```
vapi-ai-assistant/
├── public/             # Static files
├── src/                # Source code
│   ├── components/     # UI components
│   │   ├── VoiceAssistant.tsx    # Voice interface component
│   │   ├── VoiceAssistant.css    # Voice interface styles
│   │   ├── ChatInterface.tsx     # Chat interface component
│   │   └── ChatInterface.css     # Chat interface styles
│   ├── config/         # Configuration files
│   │   └── vapi.config.ts        # VAPI AI configuration
│   ├── services/       # Services 
│   │   └── vapi.service.ts       # VAPI AI service
│   ├── types/          # TypeScript types
│   │   └── vapi.types.ts         # VAPI AI related types
│   ├── App.tsx         # Main app component
│   ├── index.tsx       # Application entry point
│   └── ...             # Other files
├── .env                # Environment variables
├── package.json        # Dependencies and scripts
└── tsconfig.json       # TypeScript configuration
```

## Implementation Roadmap

This implementation follows this roadmap:

1. **Set Up VAPI AI Account**
   - Create an account on the VAPI AI platform
   - Access the dashboard to manage your projects
   - Take advantage of the free plan offering 1,000 minutes per month

2. **Build Your Voice Agent**
   - Create a new voice assistant in the VAPI AI dashboard
   - Design your conversation workflow using VAPI's workflow builder
   - Focus on crafting appropriate greeting messages
   - Upload your knowledge base documents
   - Design conversation flows for your specific use case

3. **Configure Your Voice Agent**
   - Set up the agent's voice, tone, and personality
   - Create the main prompts that guide the agent's responses
   - Test the agent through the VAPI AI testing interface

4. **Frontend Integration**
   - Add a voice call interface to your webapp
   - Implement a chat interface
   - Connect to VAPI AI using their JavaScript SDK
   - Handle call states (starting, in progress, ending)

5. **Testing and Deployment**
   - Test the voice agent thoroughly with various queries
   - Monitor response quality and adjust prompts as needed
   - Deploy the updated webapp with the integrated voice assistant

## License

MIT

## Acknowledgements

- [VAPI AI](https://vapi.ai) for providing the voice AI platform
- [React](https://reactjs.org) for the frontend framework
