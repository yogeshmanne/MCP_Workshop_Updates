## 📧 Gmail + LinkedIn Automation with MCP
Automate job applications and email handling using Cursor IDE, Pipedream, and Model Context Protocol (MCP). This project connects Gmail and LinkedIn through MCP, enabling you to apply for jobs, generate cover letters, and send personalized emails via a single prompt.


## 🧰 Tools Used
Cursor IDE – AI-powered development environment with built-in MCP interface.

Gmail & LinkedIn MCP Server – Custom Pipedream endpoints for secure data access.

Pipedream – Serverless workflow builder to manage APIs, auth, and automation logic.


## 🔧 MCP Server Configuration
Add the following configuration inside Cursor IDE > Tools and Integrations:

```json

{
  "mcpServers": {
    "Gmail Automation": {
      "url": "https://your-gmail-mcp-url.pipedream.net"
    },
    "LinkedIn Automation": {
      "url": "https://your-linkedin-mcp-url.pipedream.net"
    }
  }
}

```

 **Pro Tip** Ensure both servers are authenticated with Gmail and LinkedIn account.


## 🚀 Usage Guide
Step 1: Set Up MCP Servers
Deploy Gmail & LinkedIn MCPs via Pipedream.

Authenticate both with your accounts.

Step 2: Connect in Cursor IDE
Open Cursor IDE → Navigate to MCP tab.

Paste both MCP URLs under respective server names.

Step 3: Run the Prompt
Use the following prompt in Cursor IDE’s AI chat:

```
**Sample Prompt**
Get my details from LinkedIn, apply for a job at {company name}, write a short cover letter, and send everything to {recipient email}.
```
Customize {company name} and {recipient email} as needed.


## ✉️ What Happens Behind the Scenes
LinkedIn MCP fetches your profile and skills.

Gmail MCP drafts a custom cover letter.

Both are compiled and sent via your Gmail account to the target address.


## 🙌 Credits

Built using the Model Context Protocol and Tools mentioned.

Inspired by the NxtWave MCP Workshop


 
