# ML Learning Bytes Agent

## Overview
This project implements an AI-powered system that automatically generates and sends educational content about Machine Learning through emails. The system uses multiple specialized agents to create different types of ML learning content and delivers them in a well-formatted HTML email format.

## Features
- **ML Concept Agent**: Explains core ML concepts with definitions, analogies, and code examples
- **Interview Q&A Agent**: Generates realistic ML interview questions with structured answers
- **Mini Problem Agent**: Creates small ML coding problems with starter code
- **HTML Converter**: Formats content into professional HTML email format
- **Email Sender**: Delivers content via SendGrid email service

## Prerequisites
1. Python 3.x
2. SendGrid account (free tier available)
3. Required Python packages:
   - dotenv
   - agents
   - sendgrid
   - openai

## Setup Instructions
1. Create a SendGrid account at https://sendgrid.com/
2. Generate an API key:
   - Go to Settings >> API Keys >> Create API Key
   - Copy the key
3. Create a `.env` file in the project root with:
   ```
   SENDGRID_API_KEY=your_api_key_here
   ```
4. Verify your sender email in SendGrid:
   - Go to Settings >> Sender Authentication
   - Click "Verify a Single Sender"
   - Follow the verification process

## Project Structure
The notebook is organized into several key sections:

1. **Setup and Configuration**
   - Environment setup
   - Required imports
   - API key configuration

2. **Agent Definitions**
   - ML Concept Agent: For explaining ML concepts
   - Interview Q&A Agent: For generating interview questions
   - Mini Problem Agent: For creating coding problems
   - HTML Converter Agent: For email formatting

3. **Tool Creation**
   - Email sending functionality
   - Agent-to-tool conversions
   - Tool integration

4. **Learning Manager**
   - Main orchestrator agent
   - Content selection logic
   - Email delivery workflow

## Usage
1. Run the notebook cells in sequence
2. The system will:
   - Generate appropriate ML learning content based on user input
   - Convert content to HTML format
   - Send formatted email to specified recipient

## Customization
You can customize the system by:
1. Modifying agent instructions for different content styles
2. Adjusting email templates and formatting
3. Adding new specialized agents for different types of content
4. Changing the email sender and recipient addresses

## Notes
- Ensure your SendGrid account is properly configured
- Check spam folders if emails are not received
- The system uses GPT-4 for content generation
- HTML formatting ensures professional-looking emails

## Troubleshooting
If emails are not being received:
1. Check spam folder
2. Verify SendGrid API key
3. Confirm sender email verification
4. Check SSL certificate issues (if any)

## Contributing
Feel free to:
1. Add new types of learning content
2. Improve HTML formatting
3. Enhance email templates
4. Add more specialized agents

## License
This project is open source and available under the MIT License. 