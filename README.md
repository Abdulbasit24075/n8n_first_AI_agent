# n8n AI Agent (Beginner Project)

## Overview
This project is a simple AI agent built using **n8n**.  
The agent can receive user messages, reason using an AI model, use tools like **SerpAPI** for web search, and respond intelligently.

<img width="1920" height="932" alt="image" src="https://github.com/user-attachments/assets/8ed01d75-44ca-42ee-b666-a330f1e4ac8d" />

<img width="1394" height="914" alt="image" src="https://github.com/user-attachments/assets/a43030be-5a6a-45d0-b86d-7a3c1146475b" />

<img width="1917" height="926" alt="image" src="https://github.com/user-attachments/assets/05878dc2-f7ee-4c59-bd1b-3ff56e51bde1" />

<img width="1870" height="861" alt="image" src="https://github.com/user-attachments/assets/a90cda3f-f50e-40e9-8958-c188538e8fb8" />


## Features
- AI-powered responses using OpenAI
- Tool usage with SerpAPI (live web search)
- Short-term memory support
- Visual workflow built in n8n
-------------------------------------------------------------------------------------------------------------------------------
## Tech Stack
- n8n (Workflow Automation)
- OpenAI Chat Model
- SerpAPI
------------------------------------------------------------------------------------------------------------------------------
## How It Works
1. User sends a message
2. AI Agent analyzes the request
3. Uses tools (if needed)
4. Generates a final response
-----------------------------------------------------------------------------------------------------------------------------------
📘 Project Explanation

How This AI Agent Works

This AI agent is built using n8n and follows a simple but effective workflow.

When a user sends a message, the process starts with the “When chat message received” trigger. This trigger activates the workflow and forwards the user’s message to the AI Agent node.

AI Agent Core Components

Inside the AI Agent, three main components are used:

1. Chat Model (OpenAI Chat Model)

The agent uses an OpenAI Chat Model as its main reasoning engine.

This model understands the user’s message and decides how to respond.

Free credits provided by OpenAI were used to test and build this agent.

------------------------------------------------------------------------------------

2. Memory (Simple Memory)

The agent uses Simple Memory to maintain short-term conversation context.

This memory stores up to the last 5 messages.

It allows the agent to remember recent interactions but does not retain older messages.

This keeps the conversation context-aware while remaining lightweight.

---------------------------------------------------------------------------------------
3. Tools

The agent is connected to multiple tools to enhance its capabilities:

• Calculator   <-------------------------------

A calculator tool is included to handle mathematical calculations when required.

This was added intentionally to allow accurate numeric responses.

• SerpAPI (Web Search Tool) <----------------------------

SerpAPI is used to fetch live data from Google search results.

When a user asks a question that requires external or up-to-date information, the agent uses SerpAPI.

A private SerpAPI key is configured to securely access search results.

---------------------------------------------------------------------------------------
----------------------------
Response Flow (Step-by-Step)
The user sends a message.
The OpenAI Chat Model analyzes and understands the query.
The message is stored in Simple Memory (up to 5 recent messages).
If external information is required, the agent queries SerpAPI to fetch relevant data from Google.
The retrieved information is passed back to the OpenAI Chat Model.
The model combines its reasoning with the fetched data.
A final, intelligent response is generated and sent back to the user.
----------------------------------------------------------------------------------------------------------------------------------- 
## How to Use
🧑‍💻 How to Use This Project

1️⃣ Install or Access n8n

Sign up at https://n8n.io

Or run n8n locally using Docker

2️⃣ Import the Workflow

Open n8n dashboard

Click Import workflow

Upload the provided .json file

3️⃣ Add Required API Keys

Create an OpenAI API key

Create a SerpAPI key

Add both keys in n8n Credentials

⚠️ API keys are required for the agent to work.

4️⃣ Update Node Credentials

Open the OpenAI Chat Model node

Select your OpenAI credentials

Open the SerpAPI node

Select your SerpAPI credentials

5️⃣ Activate the Workflow

Click Save

Click Publish / Activate

6️⃣ Test the Agent

Open the Chat panel

Send a message

The AI agent will respond
## Project Status
Learning project – first AI agent built with n8n 🚀
