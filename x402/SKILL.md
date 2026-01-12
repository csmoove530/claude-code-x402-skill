---
name: x402
description: This skill should be used when the user asks to "build x402 server", "implement x402", "add x402 payments", mentions "x402 protocol", "micropayments", "paid API", "402 payment required", or discusses building monetized APIs, AI agent commerce, or payment-gated services. Activate when the user needs help with x402-based server development, integrations, or payment infrastructure.
version: 1.0.0
---

# x402 Development Skill

You are helping the user build x402-based servers and applications. x402 is a protocol for micropayments over HTTP that enables paid APIs, AI agent commerce, and monetized services.

## Your Role

When this skill is active, you should:
- Help build x402 payment servers and integrations
- Provide guidance using the resources and best practices below
- Reference the official documentation and examples when answering questions
- Suggest appropriate middleware and SDKs based on the user's tech stack
- Point users to the most relevant GitHub repositories and implementation examples

## Core Protocol & Specification

**Coinbase x402 – Overview / Welcome**
https://docs.cdp.coinbase.com/x402/docs/welcome

**x402 Foundation – Protocol site**
https://x402.org

**x402 Whitepaper**
https://x402.org/whitepaper

**x402 GitBook (spec + quickstarts)**
https://x402.gitbook.io/x402

**Coinbase x402 GitHub (reference implementation)**
https://github.com/coinbase/x402

## Seller / Server-Side Documentation

### Coinbase / CDP

**Seller Quickstart (build a paid API)**
https://docs.cdp.coinbase.com/x402/docs/seller-quickstart

**Facilitator documentation (verification + settlement model)**
https://docs.cdp.coinbase.com/x402/docs/facilitator

**x402 + MCP Server (agent-facing paid APIs)**
https://docs.cdp.coinbase.com/x402/docs/mcp-server

### thirdweb

**thirdweb x402 Server docs**
https://portal.thirdweb.com/connect/payments/x402

**thirdweb x402 Facilitator docs**
https://portal.thirdweb.com/connect/payments/x402/facilitator

**thirdweb x402 Agent / AI examples**
https://portal.thirdweb.com/ai/payments/x402

**thirdweb x402 Agent Commerce Example Repo**
https://github.com/thirdweb-example/402-agent-commerce

### DayDreams

**DayDreams x402 Nanoservice Tutorial**
https://docs.daydreams.systems/tutorials/x402-server

**AI Nanoservice with x402 Payments**
https://docs.daydreams.systems/tutorials/ai-nanoservice-x402

**DayDreams Documentation Hub**
https://docs.daydreams.systems

**DayDreams GitHub Organization**
https://github.com/daydreamsai

**Example project: lootsurvivor (x402 usage)**
https://github.com/daydreamsai/daydreams-lootsurvivor

## Explorers & Ecosystem Discovery

### x402scan

**x402scan GitHub Repository**
https://github.com/Merit-Systems/x402scan

**x402scan Ecosystem Page**
https://x402scan.com/ecosystem

The official x402scan ecosystem explorer lists actual running x402 servers on chain and their endpoints, and often links to GitHub. Look under "Node Servers (Hono, Express, Advanced)" for examples with production traffic.

### Curated lists & discovery

**awesome-x402 (Merit Systems)**
https://github.com/Merit-Systems/awesome-x402

**awesome-x402 (xpaysh)**
https://github.com/xpaysh/awesome-x402

**GitHub topic: x402**
https://github.com/topics/x402

**x402 Ecosystem Gallery**
https://x402.org/ecosystem

## Best Practices & Production Guidance

**Security considerations for x402 (community writeup)**
https://mirror.xyz/0xJasmin.eth/0cV2Zl3X9q8u2p4Zf8gF9f2k5x402-security

**Cloudflare Agents + x402 overview**
https://developers.cloudflare.com/agents/payments/x402/

**QuickNode – x402 crypto paywall tutorial**
https://www.quicknode.com/guides/web3-payments/x402-paywall

**Polygon – x402 Seller Quickstart (Express / Hono / Next)**
https://wiki.polygon.technology/docs/payments/x402/

## Middleware & SDKs (Server-Side Helpers)

**x402-fetch (buyer + server helpers)**
https://github.com/coinbase/x402-fetch

**x402 Hono middleware**
https://github.com/x402xyz/x402-hono

**Community middleware & server examples index**
https://github.com/xpaysh/awesome-x402#middleware

## Real-World / Production References

**Coinrailz production integration (discussion + code pointers)**
https://github.com/coinbase/x402/issues/44

## Major x402 Server / Protocol Repositories

These are the most prominent GitHub repositories that serve as good x402 server implementations or strong reference examples, especially those with stars, ecosystem visibility, or real usage on x402scan / ecosystem listings.

### 1) coinbase/x402 — Official reference implementation

**Repo:** https://github.com/coinbase/x402

- ⭐ **~5.2k stars** — by far the most popular & referenced x402 implementation
- Includes: core protocol, middleware for Node (Express, Hono), examples, and reference patterns for server payment gating
- Excellent base if you want to see how a production-grade protocol handles 402 responses, payload verification, and settlement logic
- A great reference server pattern — not just a library

### 2) xpaysh/awesome-x402 — Curated list of x402 ecosystem

**Repo:** https://github.com/xpaysh/awesome-x402

- ⭐ **~114 stars**
- Contains links to multiple server implementations, middleware, examples, and projects using x402
- Great place to discover well-built x402 servers and tools like Node servers, Rust, Java SDKs, and more

### 3) Merit-Systems/awesome-x402 — Another curated ecosystem list

**Repo:** https://github.com/Merit-Systems/awesome-x402

- Lower star count but broader ecosystem coverage
- Includes protocol SDKs, examples, and links to community projects that include server patterns and integrations

## Notable Language / Framework Implementations

These are less starred but solid codebases that serve as real server or middleware examples:

### 4) dabit3/a2a-x402-typescript — TypeScript x402 implementation

**Repo:** https://github.com/dabit3/a2a-x402-typescript

- ⭐ ~90+ stars
- A more complete TypeScript implementation supporting A2A (agent-to-agent) patterns with x402
- Good for seeing how server + client payment logic integrates in a real app

### 5) microchipgnu/MCPay — MCP + x402 infrastructure

**Repo:** https://github.com/microchipgnu/MCPay

- ⭐ ~78 stars
- Infrastructure that integrates x402 into MCP (Model Context Protocol) commodity services
- Useful if your server offers paid tools/services that need integrated payment gating

### 6) AIMOverse/x402-kit — SDK & modular server tooling

**Repo:** https://github.com/AIMOverse/x402-kit

- ⭐ ~50+ stars
- Offers a modular toolkit you can use to spin up x402-enabled servers
- Might include middleware and patterns that help structure server endpoints

## Rust Server Example (Production-Grade)

### 7) x402-rs/x402-rs — Rust x402 implementation + middleware

**Repo:** https://github.com/x402-rs/x402-rs

- Rust implementation with server facilitator, middleware (x402-axum), and client tooling
- Not as high star count as the Coinbase repo, but a solid server and middleware example in the Rust ecosystem
- Includes a production-ready HTTP facilitator / verification service which is essentially a server component

## Other Community Examples Worth Checking

(Not high-star but real working servers / demos which you might fork)

- **b3-fun/anyspend-x402** — multi-chain fork of the core protocol with Express server examples
  https://github.com/b3-fun/anyspend-x402

- **snc2work/x402-hono-seller-buyer-example** — minimal seller/buyer demo in Hono
  https://github.com/snc2work/x402-hono-seller-buyer-example

## Quick Summary — Best Repos to Reference

| Repository | Stars | What It Shows | Good For |
|---|---|---|---|
| https://github.com/coinbase/x402 | ⭐⭐⭐⭐⭐ | Protocol + server patterns, middleware | Official reference |
| https://github.com/xpaysh/awesome-x402 | ⭐⭐⭐ | Hub of server examples | Discovery source |
| https://github.com/dabit3/a2a-x402-typescript | ⭐⭐ | TS server + A2A payments | Real integration patterns |
| https://github.com/microchipgnu/MCPay | ⭐⭐ | Server + payment infra | MCP + x402 combos |
| https://github.com/AIMOverse/x402-kit | ⭐⭐ | SDK + server tools | Reusable server tooling |
| https://github.com/x402-rs/x402-rs | ⭐⭐ | Rust server + facilitator | Rust ecosystem example |

## Suggested Reading Order (For New Projects)

1. **Spec & flow**
   - https://docs.cdp.coinbase.com/x402/docs/welcome
   - https://x402.gitbook.io/x402

2. **Reference implementation**
   - https://github.com/coinbase/x402

3. **Server quickstart**
   - https://docs.cdp.coinbase.com/x402/docs/seller-quickstart

4. **Middleware / framework choice**
   - https://portal.thirdweb.com/connect/payments/x402
   - https://github.com/x402xyz/x402-hono

5. **Production patterns**
   - https://docs.daydreams.systems/tutorials/x402-server

## Tech Stack Recommendations

- **Express.js projects**: Use x402-fetch or custom middleware
- **Hono projects**: Use x402-hono middleware (https://github.com/x402xyz/x402-hono)
- **Next.js projects**: Follow Polygon's seller quickstart
- **AI/Agent projects**: Reference thirdweb agent examples or DayDreams tutorials
- **MCP servers**: Follow Coinbase MCP server documentation
- **TypeScript/A2A**: Check out dabit3/a2a-x402-typescript
- **Rust projects**: Use x402-rs/x402-rs

## Implementation Approach

When helping build x402 integrations:
1. Understand the user's tech stack and choose appropriate middleware
2. Follow the seller quickstart pattern for basic setup
3. Implement facilitator integration for payment verification
4. Add proper error handling and security considerations
5. Test with x402scan or ecosystem tools
6. Reference real-world examples for production patterns
7. Point to specific GitHub repos based on the tech stack and use case
