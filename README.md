# MCP
My MCP JSON-RPC Knowledge Dump


🚨 Common JSON-RPC and MCP Error Codes You Should Know 🚨

If you’re working with JSON-RPC or the Model Context Protocol (MCP), knowing these error codes can save hours of debugging.

Key error codes

-32700 Parse error. Invalid JSON

-32600 Invalid request. Wrong JSON-RPC format

-32601 Method not found. Tool or method not registered

-32602 Invalid params. Schema or type mismatch

-32603 Internal error. Server-side failure

-32000 to -32099 Custom server or application errors (very common in MCP)

💡 Rule of thumb

-326xx Protocol-level issues

-320xx Business logic or tool execution issues

Why this matters

The -326xx range is formally reserved by the JSON-RPC 2.0 specification and covers:

Invalid request structure

Method not found

Bad parameters

Internal JSON-RPC handling errors

The -32000 to -32099 range is intentionally left to the application.
In MCP implementations, it is commonly used for:

Tool execution failures

Permission or capability issues

Resource not found

Business logic errors

Mastering these distinctions makes debugging agentic AI systems and tool calling much smoother.


<img width="1659" height="936" alt="image" src="https://github.com/user-attachments/assets/e00b28b5-db87-469a-bcdb-e0daa98caec1" />

