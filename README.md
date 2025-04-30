# Multi-Tool Weather & Time Agent

A Python-based agent built with Google's ADK (Agent Development Kit) that provides weather and time information for different cities. The agent uses Gemini 2.0 Flash model for natural language processing and response generation.

## Features

- Get current weather information for cities
- Get current time in different time zones
- Natural language processing for user queries
- Built with Google's ADK and Gemini 2.0 Flash model

## Prerequisites

- Python 3.11 or higher
- Google Cloud account with Vertex AI API enabled
- Google Cloud project with appropriate credentials

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/multi_tool_agend_adk.git
cd multi_tool_agend_adk
```

2. Create and activate a virtual environment:
```bash
python -m venv .venv
source .venv/bin/activate  # On Windows, use: .venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## Configuration

1. Create a `.env` file based on the provided `.env.example`:
```bash
cp .env.example .env
```

2. Configure the following environment variables in your `.env` file:
```
GOOGLE_APPLICATION_CREDENTIALS=/path/to/your/credentials.json
GOOGLE_CLOUD_PROJECT=your-project-id
```

3. Set up Google Cloud credentials:
   - Go to Google Cloud Console
   - Create or select a project
   - Enable the Vertex AI API
   - Create a service account and download the credentials JSON file
   - Set the path to your credentials in the `.env` file

## Usage

1. Navigate to the parent directory of your agent project
```bash
cd ..\
```

1. Start the agent:
```bash
adk web
```

2. Example queries:
   - "What's the weather in New York?"
   - "What time is it in New York?"

## Project Structure

```
multi_tool_agend_adk/
├── .env.example          # Environment variables template
├── .gitignore           # Git ignore rules
├── README.md            # Project documentation
├── requirements.txt     # Python dependencies
└── multi_tool_agent/    # Main package directory
    └── agent.py         # Agent implementation
```

## Development

To contribute to the project:

1. Create a new branch:
```bash
git checkout -b feature/your-feature-name
```

2. Make your changes and commit:
```bash
git add .
git commit -m "Description of your changes"
```

3. Push your changes:
```bash
git push origin feature/your-feature-name
```

## Error Handling

Common issues and solutions:

1. Authentication Error (`invalid_grant`):
   - Verify your Google Cloud credentials are valid
   - Check if the Vertex AI API is enabled
   - Ensure your service account has proper permissions

2. Time Zone Error:
   - Verify the city name is supported
   - Check if the time zone identifier is correct

## License

MIT License

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a new Pull Request

## Support

For support, please:
1. Check the existing documentation
2. Review common error solutions in this README
3. Open an issue in the repository

## Acknowledgments

- Google ADK team for providing the agent development framework
- Contributors and maintainers of the project 