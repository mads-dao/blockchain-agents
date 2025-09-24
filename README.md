# 🚀 Claude Code Agent Collection

A comprehensive collection of specialized AI agents for Claude Code, designed to enhance development workflows across blockchain, UI/UX design, and multi-agent coordination. Built for developers who need intelligent assistance with Solana programs, blockchain documentation, Web3 frontend development, design reviews, and testing.

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
[![Open Source](https://img.shields.io/badge/Open%20Source-Yes-brightgreen)](https://opensource.org/)

## ✨ Overview

This repository contains specialized agents that extend Claude Code's capabilities across multiple domains. Each agent is an expert in a specific area, automatically invoked based on context or explicitly called when needed. All agents are configured with Claude models optimized for task complexity to deliver optimal performance and cost-effectiveness.

## 📁 Project Structure

```
blockchain-agents/
├── architect-agents/           # Documentation & Architecture
├── solana-agents/             # Solana Development & Testing
├── ui-agents/                 # Design Review & Frontend
└── list-mcp.md               # MCP Recommendations
```

## 🤖 Available Agents

### 🏗️ Architecture & Documentation

#### 📚 [Blockchain Documentation Architect](architect-agents/blockchain-documentation-architect.md)
**Purpose**: Create comprehensive technical documentation for blockchain programs and smart contracts

**Capabilities**:
- Generate detailed documentation for Solana programs and EVM smart contracts
- Create Mermaid diagrams for data flows, PDA relationships, and system architecture
- Produce sequence diagrams for transaction flows and contract interactions
- Document program-derived addresses (PDAs), account structures, and instruction handlers
- Create visual representations of complex blockchain architectures

**Best for**: Program documentation, architectural diagrams, technical specifications, onboarding materials

### ⛓️ Solana Development

#### 🧪 [Solana QA Engineer](solana-agents/solana-qa-engineer.md) 
**Purpose**: Build comprehensive test suites for Solana programs

**Capabilities**:
- Write unit tests, integration tests, and end-to-end tests
- Expert knowledge of `litesvm`, `mollusksvm`, and `solana-program-test` frameworks
- Test PDA operations, Cross-Program Invocations (CPIs), and token operations
- Create test coverage for edge cases, error conditions, and security constraints
- Migrate tests between different testing frameworks

**Best for**: Test-driven development, quality assurance, regression testing, test framework migration

#### 🎨 [Solana Web3 Frontend Architect](solana-agents/solana-web3-frontend-architect.md)
**Purpose**: Expert guidance for building production-grade Web3 frontend applications

**Capabilities**:
- Build React/Next.js components with Solana blockchain integration
- Implement wallet connection flows for multiple providers (Phantom, Solflare, etc.)
- Create robust transaction handling with error recovery and retry mechanisms
- Optimize performance with Core Web Vitals >90 and bundle size <200KB
- Develop comprehensive testing strategies (unit, integration, E2E)
- Implement PWA features and offline support
- Ensure WCAG 2.1 AA accessibility compliance

**Best for**: DApp frontend development, wallet integration, performance optimization, component architecture

### 🎨 UI/UX & Design

#### 🔍 [Design Review Agent](ui-agents/agents/design-review-agent.md)
**Purpose**: Conduct comprehensive design reviews for frontend applications

**Capabilities**:
- Automated visual testing with Playwright integration
- Comprehensive accessibility audits (WCAG 2.1 AA)
- Responsiveness testing across desktop, tablet, and mobile viewports
- Interactive state validation (hover, focus, disabled)
- Visual consistency and design system compliance
- Performance and user experience assessment

**Best for**: Pull request reviews, design system compliance, accessibility validation, visual regression testing

## 🚀 Getting Started

### Prerequisites
- [Claude Code](https://claude.ai/code) installed and configured
- Solana development environment (for Solana-specific agents)
- Rust and Anchor framework (recommended for blockchain development)
- Node.js and npm/pnpm (for frontend development)

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/blockchain-agents.git
   cd blockchain-agents
   ```

2. **Configure Claude Code agents**:
   Copy the agent configuration files to your Claude Code workspace:
   ```bash
   # Copy all agent files to your Claude Code agents directory
   cp architect-agents/*.md /path/to/your/claude-code/agents/
   cp solana-agents/*.md /path/to/your/claude-code/agents/
   cp ui-agents/agents/*.md /path/to/your/claude-code/agents/
   cp ui-agents/commands/*.md /path/to/your/claude-code/commands/
   ```

3. **Set up MCP servers** (optional but recommended):
   ```bash
   # Install recommended MCPs from list-mcp.md
   claude mcp add playwright npx @playwright/mcp@latest
   claude mcp add --transport http solana-mcp-server https://mcp.solana.com/mcp
   ```

4. **Verify installation**:
   The agents will automatically become available in Claude Code and can be invoked contextually or explicitly.

## 💡 Usage Examples

### Documentation Generation
```
user: "Document my escrow program's PDA architecture"
claude: "I'll use the blockchain-documentation-architect agent to create comprehensive documentation with Mermaid diagrams showing the PDA relationships."
```

### Test Creation
```
user: "I need tests for my new transfer_authority instruction"
claude: "I'll use the solana-qa-engineer agent to create comprehensive tests for your transfer_authority instruction using the appropriate testing framework."
```

### Frontend Development
```
user: "I need a wallet connection component that supports multiple Solana wallets"
claude: "I'll use the solana-web3-frontend-architect agent to create a robust wallet connection component with support for Phantom, Solflare, and other popular wallets."
```

### Design Review
```
user: "/design-review"
claude: "I'll conduct a comprehensive design review using Playwright to test responsiveness, accessibility, and visual consistency."
```

### Automatic Context Detection
The agents are automatically invoked when Claude Code detects relevant context:
- Creating or modifying Solana programs
- Working with blockchain documentation
- Writing or debugging tests for smart contracts
- Building React/Next.js components with Web3 integration
- Making UI/frontend changes requiring design review

## 🔧 Recommended MCPs

This project works seamlessly with Multi-Agent Coordination Protocols (MCPs) for enhanced functionality:

- **[Playwright MCP](https://github.com/microsoft/playwright-mcp)**: Browser automation for design reviews and testing
- **[Solana MCP](https://mcp.solana.com/)**: Direct Solana blockchain interaction
- **[Quicknode MCP](https://www.quicknode.com/guides/ai/quicknode-mcp)**: Blockchain infrastructure services
- **[Helius MCP](https://helius.dev/mcp)**: Enhanced Solana API services
- **[Shadcn MCP](https://ui.shadcn.com/docs/mcp)**: UI component library integration

See [list-mcp.md](list-mcp.md) for detailed installation instructions.

## 🏗️ Architecture

Each agent is designed as a specialized expert with:

- **Domain Expertise**: Deep knowledge in specific development areas
- **Tool Integration**: Seamless integration with Claude Code's tool ecosystem  
- **Context Awareness**: Automatic activation based on development context
- **Extensibility**: Easy to modify and extend for specific project needs
- **MCP Integration**: Enhanced capabilities through Multi-Agent Coordination Protocols

## 🤝 Contributing

We welcome contributions from the development community!

### How to Contribute

1. **Fork the repository**
2. **Create a feature branch**: `git checkout -b feature/new-agent`
3. **Make your changes**:
   - Add new agents to appropriate directory (`architect-agents/`, `solana-agents/`, `ui-agents/`)
   - Follow existing agent markdown format and structure
   - Update documentation and examples
   - Test your agents thoroughly
4. **Submit a pull request**

### Contribution Guidelines

- Follow the existing agent structure and formatting
- Place agents in the appropriate directory based on their domain
- Include comprehensive documentation and examples
- Test all functionality before submitting
- Update the main README.md with new agents
- Consider adding relevant MCP recommendations to `list-mcp.md`

### Ideas for New Agents

#### Blockchain & Web3
- **EVM Smart Contract Specialist**: For Ethereum/EVM development
- **Cross-Chain Bridge Expert**: For interoperability solutions  
- **DeFi Protocol Architect**: For decentralized finance applications
- **NFT Marketplace Developer**: For NFT-related functionality
- **Smart Contract Security Auditor**: For security analysis and vulnerability detection

#### Frontend & Design
- **React Performance Optimizer**: For React app optimization
- **Accessibility Specialist**: For WCAG compliance and inclusive design
- **Animation Expert**: For micro-interactions and motion design

#### DevOps & Infrastructure
- **Deployment Specialist**: For CI/CD and infrastructure automation
- **Monitoring Expert**: For observability and performance tracking

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Built for the [Claude Code](https://claude.ai/code) ecosystem
- Inspired by the Solana, blockchain, and broader development communities
- Special thanks to the teams behind Playwright, Solana, and other integrated tools
- Thanks to all contributors and users who help improve these agents

## 📞 Support

- **Issues**: Report bugs and request features via GitHub Issues
- **Discussions**: Join conversations in GitHub Discussions
- **Documentation**: Additional docs and examples available in individual agent files
- **MCP Resources**: See [list-mcp.md](list-mcp.md) for Multi-Agent Coordination Protocol setup

---

**Happy Building!** 🚀✨
