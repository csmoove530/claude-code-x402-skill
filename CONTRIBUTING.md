# Contributing to x402 Skill for Claude Code

Thank you for your interest in contributing to the x402 Claude Code skill! This document provides guidelines and instructions for contributing.

## How to Contribute

### Reporting Issues

If you encounter problems or have suggestions:

1. **Search existing issues** to avoid duplicates
2. **Create a new issue** with a clear title and description
3. **Include details:**
   - What you expected to happen
   - What actually happened
   - Steps to reproduce (if applicable)
   - Your environment (Claude Code version, OS, etc.)

### Suggesting Enhancements

We welcome suggestions for improving the skill:

- **New Resources**: Found a great x402 tutorial, example, or tool?
- **Better Organization**: Ideas for restructuring the content?
- **Framework Coverage**: Missing middleware or SDK recommendations?
- **Use Cases**: New scenarios or patterns to cover?

Open an issue with the `enhancement` label and describe your suggestion.

## Making Changes

### Setup for Development

1. **Fork the repository** on GitHub

2. **Clone your fork:**
   ```bash
   git clone https://github.com/YOUR_USERNAME/claude-code-x402-skill.git
   cd claude-code-x402-skill
   ```

3. **Create a feature branch:**
   ```bash
   git checkout -b feature/your-feature-name
   ```

4. **Install locally for testing:**
   ```bash
   cp -r x402 ~/.claude/skills/
   ```

### Skill File Structure

The skill follows the Claude Code plugin format:

```
x402/
└── SKILL.md          # Main skill definition
```

#### SKILL.md Format

The file must have YAML frontmatter:

```markdown
---
name: x402
description: Trigger conditions describing when to activate...
version: 1.0.0
---

# Skill Content

...
```

### Testing Your Changes

1. **Copy updated skill to Claude Code:**
   ```bash
   cp x402/SKILL.md ~/.claude/skills/x402/
   ```

2. **Restart Claude Code**

3. **Test activation:**
   - Try `/x402` command
   - Try natural mentions like "help me with x402"
   - Verify resources are accurate and helpful

4. **Test with different scenarios:**
   - Express.js implementation questions
   - Hono server setup
   - MCP integration
   - Rust implementation queries

### Making Good Changes

#### For Resource Additions

- **Verify links work** and point to quality content
- **Add context** - explain what the resource provides
- **Maintain organization** - put it in the right section
- **Check for duplicates** - don't add existing resources

#### For Documentation Updates

- **Be clear and concise**
- **Use proper markdown formatting**
- **Keep consistent tone** with existing content
- **Update version number** in frontmatter if significant

#### For Trigger Phrase Changes

- **Test thoroughly** - ensure skill still activates appropriately
- **Don't be too broad** - skill should activate for x402-related queries
- **Don't be too narrow** - users should find it discoverable

### Commit Guidelines

Write clear, descriptive commit messages:

```bash
# Good
git commit -m "Add thirdweb x402 Agent Commerce examples"
git commit -m "Fix broken link to Coinbase facilitator docs"
git commit -m "Update Hono middleware recommendation"

# Not as good
git commit -m "Update"
git commit -m "Fix stuff"
git commit -m "Changes"
```

### Submitting Pull Requests

1. **Push your changes:**
   ```bash
   git push origin feature/your-feature-name
   ```

2. **Create a Pull Request** on GitHub

3. **Describe your changes:**
   - What does this PR do?
   - Why is it needed?
   - How was it tested?
   - Related issues (if any)

4. **Wait for review** - maintainers will review and provide feedback

## Content Guidelines

### Adding Documentation Links

When adding new documentation or resources:

- **Prefer official sources** (x402.org, Coinbase docs, framework docs)
- **Include star counts** for GitHub repos (helps users gauge popularity)
- **Add brief descriptions** explaining what each resource provides
- **Organize by category** (Core Protocol, Framework-Specific, Examples, etc.)

### Writing Implementation Guidance

- **Be framework-specific** when applicable
- **Link to examples** rather than including full code in the skill
- **Highlight best practices** and security considerations
- **Keep it actionable** - users should know what to do next

### Maintaining Quality

- **Test all links** before submitting
- **Update outdated information** when found
- **Remove deprecated resources** if better alternatives exist
- **Keep descriptions accurate** and helpful

## Code of Conduct

### Our Standards

- **Be respectful** and inclusive
- **Be constructive** in feedback and criticism
- **Focus on what's best** for the community
- **Show empathy** towards other contributors

### Unacceptable Behavior

- Harassment, discrimination, or offensive comments
- Trolling or deliberately disruptive behavior
- Publishing others' private information
- Other conduct inappropriate in a professional setting

## Questions?

- **General questions**: Open a GitHub issue
- **Security concerns**: Email the maintainer directly
- **Quick clarifications**: Comment on relevant issues or PRs

## Recognition

Contributors will be recognized in the project:
- Your GitHub username in the contributors list
- Acknowledgment in the README for significant contributions
- Appreciation from the community for improving the skill

## License

By contributing, you agree that your contributions will be licensed under the MIT License.

---

Thank you for contributing to make x402 development with Claude Code better!
