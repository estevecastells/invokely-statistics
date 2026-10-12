# Invokely Statistics for Gemini CLI

This extension configures Gemini CLI to use Invokely's hosted MCP server over Streamable HTTP. It provides six statistics tools: search indicators, resolve places, retrieve values, read full series, compare places, and rank locations.

The manifest uses Gemini CLI's documented `includeTools` setting to expose those six statistics operations. Invokely's hosted server also lists workspace tools, but this extension does not expose workspace list, read, save, update, or delete operations. See [Invokely's developer documentation](https://invokely.ai/docs) and [current pricing](https://invokely.ai/pricing) for current service details.

## Install

Install this extension from a terminal:

```sh
gemini extensions install https://github.com/estevecastells/invokely-statistics
```

After installation, restart Gemini CLI and use the Invokely MCP tools in your session. This configuration uses the no-account trial endpoint and requires no Invokely API key. The trial allows 25 calls per day per IP. A separate registered Free plan includes 500 MCP calls per month. The extension does not include Invokely's hosted backend or configure the REST API.

The extension follows Gemini CLI's documented remote MCP and tool-filter configuration. It is a third-party integration and is not endorsed by Google. The local MIT-licensed stdio adapter is available separately at [invokely-mcp-connector](https://github.com/estevecastells/invokely-mcp-connector).
