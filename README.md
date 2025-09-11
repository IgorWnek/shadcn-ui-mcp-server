# Shadcn UI v4 MCP Server

[![npm version](https://badge.fury.io/js/@jpisnice%2Fshadcn-ui-mcp-server.svg)](https://badge.fury.io/js/@jpisnice%2Fshadcn-ui-mcp-server)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

[![Trust Score](https://archestra.ai/mcp-catalog/api/badge/quality/Jpisnice/shadcn-ui-mcp-server)](https://archestra.ai/mcp-catalog/jpisnice__shadcn-ui-mcp-server)

> **🚀 The fastest way to integrate shadcn/ui components into your AI workflow**

A Model Context Protocol (MCP) server that provides AI assistants with comprehensive access to [YashTellis/ui](https://github.com/YashTellis/ui) components, blocks, demos, and metadata. Seamlessly retrieve React, Svelte, and Vue implementations for your AI-powered development workflow.

## ✨ Key Features

- **🎯 Multi-Framework Support** - React, Svelte, and Vue implementations
- **📦 Component Source Code** - Latest YashTellis/ui v4 TypeScript source
- **🎨 Component Demos** - Example implementations and usage patterns  
- **🏗️ Blocks Support** - Complete block implementations (dashboards, calendars, forms)
- **📋 Metadata Access** - Dependencies, descriptions, and configuration details
- **🔍 Directory Browsing** - Explore repository structures
- **🚀 Component Creation** - Generate new components following existing patterns
- **📤 Component Push** - Push created components back to UI repositories (with GitHub token)
- **⚡ Smart Caching** - Efficient GitHub API integration with rate limit handling

## 🚀 Quick Start

```bash
# Basic usage (60 requests/hour)
npx @jpisnice/shadcn-ui-mcp-server

# With GitHub token (5000 requests/hour) - Recommended
npx @jpisnice/shadcn-ui-mcp-server --github-api-key ghp_your_token_here

# Switch frameworks
npx @jpisnice/shadcn-ui-mcp-server --framework svelte
npx @jpisnice/shadcn-ui-mcp-server --framework vue
```

**🎯 Get your GitHub token in 2 minutes**: [docs/getting-started/github-token.md](docs/getting-started/github-token.md)

## 📚 Documentation

| Section | Description |
|---------|-------------|
| [🚀 Getting Started](docs/getting-started/) | Installation, setup, and first steps |
| [⚙️ Configuration](docs/configuration/) | Framework selection, tokens, and options |
| [🔌 Integration](docs/integration/) | Editor and tool integrations |
| [📖 Usage](docs/usage/) | Examples, tutorials, and use cases |
| [🎨 Frameworks](docs/frameworks/) | Framework-specific documentation |
| [🐛 Troubleshooting](docs/troubleshooting/) | Common issues and solutions |
| [🔧 API Reference](docs/api/) | Tool reference and technical details |

## 🎨 Framework Support

This MCP server supports three popular shadcn implementations:

| Framework | Repository | Maintainer | Description |
|-----------|------------|------------|-------------|
| **React** (default) | [YashTellis/ui](https://github.com/YashTellis/ui) | [YashTellis](https://github.com/YashTellis) | React components from YashTellis/ui v4 |
| **Svelte** | [shadcn-svelte](https://www.shadcn-svelte.com/) | [huntabyte](https://github.com/huntabyte) | Svelte components from shadcn-svelte |
| **Vue** | [shadcn-vue](https://www.shadcn-vue.com/) | [unovue](https://github.com/unovue) | Vue components from shadcn-vue |

## 🏗️ Essential Setup

### 1. Get GitHub Token (Required for Push Operations)
```bash
# Visit: https://github.com/settings/tokens
# Generate token with 'Contents: Write' permission for push operations
# No scopes needed for read-only operations
export GITHUB_PERSONAL_ACCESS_TOKEN=ghp_your_token_here
```

**🔒 Important**: For pushing components to repositories, your GitHub token needs:
- **Contents: Write** permission
- Access to the target repository (fork or direct access)
- For private repositories: appropriate repository access

### 2. Run Server
```bash
# React (default)
npx @jpisnice/shadcn-ui-mcp-server

# Svelte
npx @jpisnice/shadcn-ui-mcp-server --framework svelte

# Vue  
npx @jpisnice/shadcn-ui-mcp-server --framework vue
```

### 3. Integrate with Your Editor
- **VS Code**: [docs/integration/vscode.md](docs/integration/vscode.md)
- **Cursor**: [docs/integration/cursor.md](docs/integration/cursor.md)
- **Claude Desktop**: [docs/integration/claude-desktop.md](docs/integration/claude-desktop.md)
- **Continue.dev**: [docs/integration/continue.md](docs/integration/continue.md)

## 🎯 Use Cases

- **AI-Powered Development** - Let AI assistants build UIs with YashTellis/ui
- **Component Discovery** - Explore available components and their usage
- **Multi-Framework Learning** - Compare React, Svelte, and Vue implementations
- **Rapid Prototyping** - Get complete block implementations for dashboards, forms, etc.
- **Code Generation** - Generate component code with proper dependencies
- **Component Contribution** - Create and push new components back to UI repositories
- **Repository Management** - Manage component libraries through AI workflows

## 📦 Installation

```bash
# Global installation (optional)
npm install -g @jpisnice/shadcn-ui-mcp-server

# Or use npx (recommended)
npx @jpisnice/shadcn-ui-mcp-server
```

## 🔗 Quick Links

- 📖 [Full Documentation](docs/)
- 🚀 [Getting Started Guide](docs/getting-started/)
- 🎨 [Framework Comparison](docs/frameworks/)
- 🔧 [API Reference](docs/api/)
- 🐛 [Troubleshooting](docs/troubleshooting/)
- 💬 [Issues & Discussions](https://github.com/Jpisnice/shadcn-ui-mcp-server)

## 📄 License

MIT License - see [LICENSE](LICENSE) for details.

## 🙏 Acknowledgments

- **[YashTellis](https://github.com/YashTellis)** - For the React UI component library
- **[huntabyte](https://github.com/huntabyte)** - For the excellent Svelte implementation
- **[unovue](https://github.com/unovue)** - For the comprehensive Vue implementation
- **[Anthropic](https://anthropic.com)** - For the Model Context Protocol specification

---

**Made with ❤️ by [Janardhan Polle](https://github.com/Jpisnice)**

**Star ⭐ this repo if you find it helpful!**
