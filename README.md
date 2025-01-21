# Financial and Web Search AI Agents

This project showcases the integration of advanced AI agents designed for financial analysis and web search functionalities. It uses the `phi` framework to create specialized agents capable of leveraging tools like YFinance and DuckDuckGo to provide users with actionable insights.

## Table of Contents
1. [Overview](#overview)
2. [Features](#features)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Agents](#agents)
6. [Playground](#playground)
7. [Environment Variables](#environment-variables)
8. [Dependencies](#dependencies)
9. [Contributing](#contributing)
10. [License](#license)

## Overview

This repository contains two main agents:
- **Web Search Agent**: Designed to perform web searches and fetch information using DuckDuckGo.
- **Finance AI Agent**: Provides financial insights such as stock prices, analyst recommendations, company news, and stock fundamentals using YFinance.

Both agents are designed to interact seamlessly and provide results in an intuitive format like tables, with a strong emphasis on user-friendly outputs.

## Features

### Financial Data Analysis
- Fetch stock prices, analyst recommendations, and financial fundamentals
- Summarize the latest company news

### Web Search
- Search the web for information with source citations

### Multi-agent Collaboration
- Combine agents for comprehensive outputs

### Interactive Playground
- Host and interact with agents via a user-friendly FastAPI playground

## Installation

1. Clone the repository:
```bash
git clone https://github.com/your-repo-name.git
cd your-repo-name
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Set up environment variables:
   - Create a `.env` file in the root directory with:
```
OPENAI_API_KEY=your_openai_api_key
PHI_API_KEY=your_phi_api_key
```

## Usage

### Running the Financial Agent
Use the `financial_agent.py` script to execute predefined queries:
```bash
python financial_agent.py
```

### Launching the Playground
Start the interactive playground using the `playground.py` script:
```bash
python playground.py
```
Access the playground at `http://127.0.0.1:8000`.

## Agents

### Web Search Agent
- **Role**: Fetches web information
- **Tools**: DuckDuckGo
- **Features**:
  - Includes source citations
  - Outputs results in markdown format

### Finance AI Agent
- **Role**: Performs financial analysis
- **Tools**: YFinance
- **Features**:
  - Displays financial data in tables
  - Fetches stock prices, fundamentals, recommendations, and news

## Playground
The project includes an interactive playground powered by FastAPI, where users can interact with the agents. The playground provides a graphical interface for running queries and visualizing results.

## Environment Variables
Ensure the following environment variables are set in a `.env` file:
- `OPENAI_API_KEY`: API key for OpenAI integration
- `PHI_API_KEY`: API key for the Phi framework

## Dependencies
The project uses the following Python packages:
- `phidata`: Core framework for building AI agents
- `python-dotenv`: For loading environment variables
- `yfinance`: Fetching financial data
- `duckduckgo-search`: Web search functionality
- `fastapi` and `uvicorn`: Hosting the interactive playground
- `groq`: Model integration for advanced AI capabilities
- `openai`: OpenAI API integration

Install all dependencies using:
```bash
pip install -r requirements.txt
```

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request with your proposed changes.

## License
This project is licensed under the MIT License. See the LICENSE file for details.
