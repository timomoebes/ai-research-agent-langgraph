# 🔍 Advanced Developer Tools Research Agent

An intelligent AI agent that researches and analyzes developer tools, frameworks, and technologies using advanced web scraping, LLM analysis, and structured workflows. Built with ❤️ using LangGraph, OpenAI, and Firecrawl.

## ✨ Features

- **🔍 Smart Tool Discovery**: Automatically extracts relevant tools from web articles and documentation
- **🧠 Intelligent Analysis**: Structured analysis using OpenAI's GPT-4o-mini with custom prompts
- **🌐 Comprehensive Web Scraping**: Powered by Firecrawl for reliable content extraction
- **📊 Structured Data Output**: Pydantic models ensure consistent, parseable results
- **🔄 Multi-Step Workflow**: LangGraph orchestrates complex research workflows
- **💡 Contextual Recommendations**: Provides actionable insights based on comprehensive analysis

## 🚀 Installation

1. **📥 Clone the repository**:
   ```bash
   git clone https://github.com/timomoebes/ai-research-agent-langgraph.git
   cd ai-research-agent-langgraph/advanced-agent
   ```

2. **📦 Install dependencies**:
   ```bash
   uv sync
   ```

3. **⚙️ Set up environment variables**:
   ```bash
   cp .env.example .env
   # Edit .env with your API keys
   ```

   Required variables:
   ```env
   OPENAI_API_KEY=your_openai_api_key_here
   FIRECRAWL_API_KEY=your_firecrawl_api_key_here
   ```

## 🚀 Usage

Run the agent:
```bash
python -m uv run main.py
```

**🔍 Example Queries**:
- `"Windsurf"` - Research the Windsurf code editor
- `"React state management"` - Find React state management solutions
- `"database ORM"` - Discover database ORM libraries
- `"API documentation tools"` - Research API documentation platforms

**📝 Sample Output**:
```
= Developer Tools Research Agent

Developer Tools Query: Windsurf
= Finding articles about: Windsurf
Extracted tools: Windsurf, VS Code, Cursor, Zed, Sublime Text
Researching specific tools: Windsurf, VS Code, Cursor, Zed
```

## 📂 Project Structure

```
advanced-agent/
├── main.py                 # Application entry point
├── src/
│   ├── __init__.py
│   ├── workflow.py         # LangGraph workflow orchestration
│   ├── models.py           # Pydantic data models
│   ├── prompts.py          # LLM prompt templates
│   └── firecrawl.py        # Web scraping service
├── pyproject.toml          # Project configuration
└── README.md               # This file
```

## ⚙️ Configuration

### 🔑 Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `OPENAI_API_KEY` | OpenAI API key for LLM access | ✓ |
| `FIRECRAWL_API_KEY` | Firecrawl API key for web scraping | ✓ |
| `OPENAI_MODEL_NAME` | OpenAI model (default: gpt-4o-mini) | |

## 📜 License

MIT License - see LICENSE file for details.

## 🙏 Acknowledgments

- **[LangGraph](https://langchain-ai.github.io/langgraph/)**: Workflow orchestration
- **[OpenAI](https://openai.com/)**: Language model capabilities
- **[Firecrawl](https://firecrawl.dev/)**: Web scraping infrastructure
- **[Pydantic](https://pydantic.dev/)**: Data validation and serialization
