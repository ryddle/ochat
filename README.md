# OChat - Ollama Web Client

OChat is a web-based client interface for interacting with Ollama language models. It provides a clean and intuitive interface for managing chat conversations with different AI models.

## Features

- **Model Selection**: Choose from available Ollama models
- **Chat Management**: 
  - Create new chats
  - Save chats locally in browser storage
  - Export chats to external server (configurable)
  - Delete chats
  - Rename chats
  - Switch between multiple chats

- **Chat Interface**:
  - Real-time streaming responses
  - Markdown support in AI responses
  - Code syntax highlighting
  - Support for ordered and unordered lists
  - Code block formatting

- **Upcoming Features**:
  - File attachments support
  - Voice input through speech recognition

## Requirements

- Ollama running locally on port 11434
- Modern web browser with localStorage support
- Optional: External server for chat exports

## Setup

1. Ensure Ollama is running locally
2. Open index.html in a web browser
3. Select your preferred model from the dropdown
4. Start chatting!

## Chat Export Configuration

To enable chat exports, configure your server endpoint in the `saveToServer()` function:

```javascript
fetch(`http://your-server/path/${filename}`, requestOptions)
```

## Technical Details

- Built with vanilla JavaScript
- Uses browser's localStorage for chat persistence
- Implements server-sent events for streaming responses
- Uses Prism.js for code syntax highlighting

## Browser Compatibility

Works with modern browsers that support:
- Web Speech API
- Fetch API
- localStorage
- ES6+ features

## License

MIT

## Contributing

Feel free to open issues or submit pull requests for improvements.