# Financial Researcher Project using CrewAI

This project implements an intelligent financial research system using CrewAI agents to perform comprehensive market analysis and generate insights.

## Project Overview

The Financial Researcher is built using CrewAI, a framework that enables the creation of multiple AI agents working together to accomplish complex tasks. This project demonstrates how different specialized agents can collaborate to perform financial research and analysis.

## Agent Workflow

The project utilizes two specialized agents working in coordination:

1. **Senior Financial Researcher**
   - Conducts in-depth financial analysis
   - Evaluates market trends and patterns
   - Provides expert financial insights
   - Makes investment recommendations

2. **Market Analyst and Report Writer**
   - Gathers and analyzes market data
   - Identifies market opportunities and risks
   - Compiles comprehensive research reports
   - Formats findings for clarity and readability

## Prerequisites

### API Requirements

1. **Serper API Key**
   - Required for web search capabilities
   - Sign up at [Serper.dev](https://serper.dev)
   - Set as environment variable: `SERPER_API_KEY`

### Required Libraries

Install the following Python packages:

```bash
pip install crewai
pip install python-dotenv
```

## Project Setup

1. **Create Project Structure**

```bash
mkdir financial_researcher
cd financial_researcher
```

2. **Set Up Virtual Environment**

```bash
python -m venv venv
source venv/bin/activate  # On Windows: .\venv\Scripts\activate
```

3. **Environment Configuration**

Create a `.env` file in the project root:

```plaintext
SERPER_API_KEY=your_serper_api_key_here
OPENAI_API_KEY=your_openai_api_key_here
```

```

## Running the Project

1. **Navigate to the Project Directory**

```bash
cd src/financial_researcher
```

2. **Execute the Main Script**

```bash
crewai run
```

The agents will begin their collaborative research process and generate a report in the `output/report.md` file.

## Customization

You can customize the research parameters and agent behaviors by modifying:

- `knowledge/user_preference.txt` - Set user-specific research preferences
- `src/financial_researcher/config/` - Adjust agent configurations
- `src/financial_researcher/tools/` - Add or modify research tools
