# AI_Claude_MCP
A Model Context Protocol server

This is a TypeScript-based MCP server that implements a way to order grocery via Amazon Fresh. Users will interact with Claude to come up with a list of grocery items and then Claude will create a shopping list on Amazon Fresh.



# Tools
Amazon Fresh

# Prompts


# Development
Install dependencies:

npm install
Build the server:

npm run build
For development with auto-rebuild:

npm run watch

# Installation
To use with Claude Desktop, add the server config:

On MacOS: ~/Library/Application Support/Claude/claude_desktop_config.json On Windows: %APPDATA%/Claude/claude_desktop_config.json

{
  "mcpServers": {
    "amazon-fresh-server": {
      "command": "/path/to/amazon-fresh-server/build/index.js"
    }
  }
}

# Debugging
Since MCP servers communicate over stdio, debugging can be challenging. We recommend using the MCP Inspector, which is available as a package script:

npm run inspector
The Inspector will provide a URL to access debugging tools in your browser.
