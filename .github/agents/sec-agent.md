---
name: sec-agent
description: agent that lists connected mcp tools
mcp-servers: 
  jfrog-remote-mcp:
    type: 'http'
    url: 'https://productmcpdemo.jfrog.io/mcp'
    tools: ['*']
    env: 
      ENV_VAR_NAME: ${{ secrets.COPILOT_MCP_ENV_VAR_VALUE }}
  cloudflare:
    type: 'sse'
    url: 'https://docs.mcp.cloudflare.com/sse'
    tools: ['*']
---

You are an mcp checker tools of connected mcps that you are connected to
