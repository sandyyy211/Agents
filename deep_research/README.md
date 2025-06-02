# Deep Research

A sophisticated AI-powered research assistant that performs comprehensive web research on any topic and generates detailed reports.

## Overview

Deep Research is an intelligent research system that combines multiple AI agents to:
- Plan and execute targeted web searches
- Analyze and synthesize information
- Generate comprehensive research reports
- Deliver results via email

## Features

- **Intelligent Search Planning**: Automatically breaks down research topics into targeted search queries
- **Parallel Search Execution**: Performs multiple searches concurrently for efficient research
- **Comprehensive Reporting**: Generates well-structured, detailed research reports
- **Email Delivery**: Sends research results directly to your inbox
- **Web Interface**: User-friendly Gradio interface for easy interaction
- **Traceable Execution**: View detailed execution traces for transparency

## Installation

1. Clone the repository:
```bash
git clone [repository-url]
cd deep_research
```

2. Install required Python packages:
```bash
pip install gradio python-dotenv openai
```

3. Set up environment variables:
Create a `.env` file with your configuration:
```
[Add required environment variables]
```
4. Create a SendGrid account at https://sendgrid.com/
Generate an API key:
Go to Settings >> API Keys >> Create API Key
Copy the key
Create a .env file in the project root with:
SENDGRID_API_KEY=your_api_key_here
Also, add OPENAI_API_KEY in env file
Verify your sender email in SendGrid:
Go to Settings >> Sender Authentication
Click "Verify a Single Sender"
Follow the verification process

## Usage

1. Start the web interface:
```bash
python deep_research.py
```

2. Open your browser and navigate to the provided local URL
3. Enter your research topic in the text box
4. Click "Run" or press Enter to start the research process
5. View the progress and final report in the interface
6. Check your email for the complete research report

## Project Structure

- `deep_research.py`: Main application entry point and web interface
- `research_manager.py`: Core research orchestration logic
- `planner_agent.py`: Search planning agent
- `search_agent.py`: Web search execution agent
- `writer_agent.py`: Report generation agent
- `email_agent.py`: Email delivery agent

## Requirements

- Python 3.8+
- Required Python packages:
  - gradio: For the web interface
  - python-dotenv: For environment variable management
  - openai: For AI model interactions
- OpenAI API access
- Internet connection for web searches
- Email configuration for report delivery
