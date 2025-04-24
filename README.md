# AgenticAI

A Python-based project demonstrating the power of AI agents built using OpenAI's API. This project showcases how to create and orchestrate multiple AI agents to perform complex tasks like translation and content generation.

## Features

- 🤖 Multiple AI Agents: Create specialized agents for different tasks
- 🔄 Async Support: Built with asyncio for efficient concurrent operations
- 🌐 Translation Capabilities: Multi-language translation support
- 🎯 Task Orchestration: Coordinate multiple agents to work together
- 📝 Content Generation: Generate creative content like haikus and translations

## Prerequisites

- Python 3.13 or higher
- OpenAI API key
- pip (Python package manager)

## Installation

1. Clone the repository:
```bash
git clone url
cd AgenticAI
```

2. Create and activate a virtual environment:
```bash
python -m venv env
source env/bin/activate  # On Windows, use: env\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Set up your OpenAI API key:
```bash
export OPENAI_API_KEY='your-api-key-here'
```

## Usage

### Basic Translation Example

Run the translation example:
```bash
python AIAgents-OpenAI.py
```

The script will prompt you to:
1. Enter the text you want to translate
2. Specify the target language
3. Receive the translation output

### Creating Custom Agents

You can create your own agents by modifying the `AIAgents-OpenAI.py` file:

```python
from agents import Agent, Runner

# Create a specialized agent
my_agent = Agent(
    name="my_agent",
    instructions="Your custom instructions here"
)

# Use the agent
result = await Runner.run(my_agent, "Your prompt here")
```

## Project Structure

- `AIAgents-OpenAI.py`: Main example file demonstrating agent usage
- `agents/`: Core agent implementation (imported from the agents package)
- `requirements.txt`: Project dependencies

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- OpenAI for providing the powerful API
- The agents package for the agent framework