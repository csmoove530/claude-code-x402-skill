# x402 Skill for Claude Code

A Claude Code skill that provides expert guidance for building x402-based servers and applications. x402 is a protocol for micropayments over HTTP that enables paid APIs, AI agent commerce, and monetized services.

## What is This?

This is a **Claude Code Skill** - a specialized knowledge module that automatically activates when you're working with x402 protocol implementations. When active, Claude will have instant access to:

- Comprehensive x402 documentation and resources
- Best practices for server implementation
- Framework-specific middleware recommendations
- Production-ready examples and reference implementations
- Security considerations and patterns

## Features

- **Automatic Activation**: The skill activates when you mention x402, paid APIs, micropayments, or related concepts
- **Framework Recommendations**: Get middleware suggestions based on your tech stack (Express, Hono, Next.js, Rust, etc.)
- **Curated Resources**: Access to the best x402 repositories, tutorials, and documentation
- **Implementation Guidance**: Step-by-step help for building x402 payment servers
- **Production Patterns**: Real-world examples and best practices

## Installation

### Prerequisites

- [Claude Code](https://github.com/anthropics/claude-code) CLI installed (version 2.0+)

### Quick Install

1. **Clone this repository:**
   ```bash
   git clone https://github.com/csmoove530/claude-code-x402-skill.git
   ```

2. **Copy the skill to your Claude Code skills directory:**
   ```bash
   cp -r claude-code-x402-skill/x402 ~/.claude/skills/
   ```

3. **Verify installation:**
   ```bash
   ls ~/.claude/skills/x402/
   # Should show: SKILL.md
   ```

4. **Restart Claude Code** for the skill to be recognized.

### Manual Installation

If you prefer to install manually:

1. Create the skill directory:
   ```bash
   mkdir -p ~/.claude/skills/x402
   ```

2. Download the skill file:
   ```bash
   curl -o ~/.claude/skills/x402/SKILL.md \
     https://raw.githubusercontent.com/csmoove530/claude-code-x402-skill/main/x402/SKILL.md
   ```

3. Restart Claude Code.

## Usage

### Method 1: Slash Command (Recommended)

Simply type `/x402` in your Claude Code conversation:

```
You: /x402 - I want to build a paid API using Express.js

Claude: [Activates x402 skill and provides Express.js-specific guidance with
middleware recommendations, code examples, and best practices]
```

### Method 2: Natural Mention

Just mention x402 or related concepts in your conversation:

```
You: Help me implement x402 payments for my Next.js app

Claude: [Automatically activates the skill and provides Next.js-specific guidance]
```

### Trigger Phrases

The skill activates when you mention:
- "build x402 server"
- "implement x402"
- "add x402 payments"
- "x402 protocol"
- "micropayments"
- "paid API"
- "402 payment required"
- "monetized APIs"
- "AI agent commerce"
- "payment-gated services"

## What You'll Get

When the skill is active, Claude will help you with:

### 1. Tech Stack Recommendations
- **Express.js**: x402-fetch or custom middleware
- **Hono**: x402-hono middleware
- **Next.js**: Polygon's seller quickstart patterns
- **AI/Agent projects**: thirdweb and DayDreams examples
- **MCP servers**: Coinbase MCP integration patterns
- **Rust**: x402-rs implementation and middleware

### 2. Resource Access
The skill includes links to:
- Official x402 documentation (Coinbase, x402.org)
- Framework-specific middleware and SDKs
- Production examples and reference implementations
- Security best practices
- Ecosystem tools (x402scan, awesome-x402 lists)

### 3. Implementation Guidance
Step-by-step help with:
- Setting up payment-gated endpoints
- Integrating facilitator services
- Implementing proper error handling
- Testing with x402scan
- Deploying to production

## Examples

### Building an Express.js Paid API

```
You: /x402 - Build me a paid API endpoint with Express.js

Claude: I'll help you create an x402-enabled Express.js server. Based on your
stack, I recommend using x402-fetch middleware...

[Provides complete implementation with code examples, configuration, and testing steps]
```

### Adding x402 to a Hono Server

```
You: I have a Hono server and want to add x402 payments

Claude: For Hono servers, the x402-hono middleware is your best option...

[Provides Hono-specific implementation with middleware setup and examples]
```

### Creating an MCP Server with Payments

```
You: /x402 - How do I create an MCP server with paid tool access?

Claude: For MCP servers with x402 payments, Coinbase provides excellent
documentation. Let me walk you through the setup...

[Provides MCP-specific guidance with tool configuration and payment integration]
```

## Skill Content Overview

The skill provides access to:

- **Core Protocol Documentation**: Official specs, whitepapers, and protocol sites
- **Seller/Server Documentation**: Quickstarts for Coinbase, thirdweb, and DayDreams
- **Ecosystem Discovery**: x402scan, awesome-x402 lists, production examples
- **Best Practices**: Security considerations, production patterns, deployment guides
- **Major Repositories**: Curated list of the best x402 implementations and examples
- **Framework Integration**: Language and framework-specific guidance

## Verification

To verify the skill is installed correctly:

1. Start Claude Code
2. Type `/x402` or mention "x402 protocol"
3. Claude should recognize the trigger and activate the skill
4. You'll receive x402-specific guidance and resource recommendations

## Troubleshooting

### Skill Not Activating

1. **Check file structure:**
   ```bash
   ls -la ~/.claude/skills/x402/
   # Should show SKILL.md with proper permissions
   ```

2. **Verify file format:**
   ```bash
   head -5 ~/.claude/skills/x402/SKILL.md
   # Should show YAML frontmatter with --- delimiters
   ```

3. **Restart Claude Code:**
   - Exit current session
   - Start a new session
   - Try activating again with `/x402`

### File Permission Issues

```bash
chmod 644 ~/.claude/skills/x402/SKILL.md
```

## Contributing

Contributions are welcome! Here's how you can help:

### Reporting Issues
- Found outdated links or resources? Open an issue
- Skill not activating properly? Let us know your setup
- Missing important x402 resources? Suggest additions

### Submitting Changes
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/add-resource`)
3. Update `x402/SKILL.md` with your changes
4. Test the skill locally
5. Submit a pull request

See [CONTRIBUTING.md](CONTRIBUTING.md) for detailed guidelines.

## Resources

### Official x402 Links
- [x402.org](https://x402.org) - Protocol site
- [Coinbase x402 Docs](https://docs.cdp.coinbase.com/x402/docs/welcome) - Official documentation
- [x402 GitBook](https://x402.gitbook.io/x402) - Specifications and quickstarts

### Community Resources
- [awesome-x402 (xpaysh)](https://github.com/xpaysh/awesome-x402) - Curated ecosystem list
- [awesome-x402 (Merit Systems)](https://github.com/Merit-Systems/awesome-x402) - Another great list
- [x402scan](https://x402scan.com/ecosystem) - Ecosystem explorer

## License

MIT License - see [LICENSE](LICENSE) file for details.

## Acknowledgments

This skill aggregates resources from the x402 community, including:
- Coinbase and the x402 protocol team
- thirdweb for agent commerce patterns
- DayDreams for nanoservice tutorials
- Merit Systems for x402scan ecosystem explorer
- All contributors to awesome-x402 lists

## About Claude Code Skills

Claude Code Skills are specialized knowledge modules that enhance Claude's ability to help with specific domains. Learn more about creating skills in the [Claude Code documentation](https://github.com/anthropics/claude-code).

---

**Built with Claude Code** | [Report Issues](https://github.com/csmoove530/claude-code-x402-skill/issues) | [View Source](https://github.com/csmoove530/claude-code-x402-skill)
