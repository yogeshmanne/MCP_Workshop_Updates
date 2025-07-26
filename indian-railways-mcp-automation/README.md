# 🚆 Indian Railways MCP Automation

This project demonstrates how to automate real-time Railway information retrieval using **Cursor IDE**, **Pipedream**, and the **Model Context Protocol (MCP)**. The automation is powered by an MCP server configured for the Indian Railways and allows querying schedules, seat availability, and live train status through natural language prompts.


## 🧠 Tools Used

- **Cursor IDE** – An AI-driven development environment with native MCP support.
- **Indian Railways MCP Server** – Custom endpoint to fetch real-time railway data.
- **Pipedream** – (Optional) For workflow orchestration and webhook-based triggers.



## ⚙️ MCP Configuration in Cursor IDE

Add the following snippet to your **Cursor IDE > Tools and Integrations** to configure the Indian Railways MCP server:

```json
{
  "mcpServers": {
    "Indian Railway": {
      "url": "https://railway-mcp.amithv.xyz/mcp"
    }
  }
}

```


## 🚀 How It Works
1. Open Cursor IDE and navigate to the Chat.
2. Write a Prompt.
   
   Example Prompt :
   Give me the list of Trains from Hyderabad to Tirupati on 2025-07-28.

3. The MCP server will return the train schedule for the requested route and date.


## 🙌 Credits
Indian Railways MCP by @amithv

Workshop conducted by Nxtwave - MCP 
