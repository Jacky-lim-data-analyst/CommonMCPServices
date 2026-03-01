# MCP Servers
A collection of [Model Context Protocol (MCP)](https://modelcontextprotocol.io/docs/getting-started/intro) servers implemented in multiple languages.

## Languages

| Language | Directory |
|----------|-----------|
| Python   | [`python/`](./python) |
| Go       | [`golang/`](./golang) |

## What is MCP?

MCP is an open protocol that standardizes how applications provide context to LLMs. MCP servers expose tools, resources, and prompts that AI clients (like Claude) can discover and use.

## Project structure
```
mcp_servers/
├── python/
│   ├── pyproject.toml
│   ├── uv.lock
│   ├── README.md
│   ├── servers/
│   │   ├── weather/
│   ├── shared/
│   └── tests/
└── golang/
```

## Getting Started

### Python

Requires Python 3.11+ and [uv](https://docs.astral.sh/uv/).

```bash
cd python
uv sync
```

To run a specific server:

```bash
uv run python servers/filesystem/server.py
```

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feat/my-new-server`)
3. Commit your changes
4. Open a pull request

## License
[MIT](./LICENSE)
