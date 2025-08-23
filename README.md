# 🚀 Claude Code Blockchain Subagents Collection

A comprehensive collection of specialized AI subagents for Claude Code, designed to enhance blockchain development workflows with domain-specific expertise. Built for developers who need intelligent assistance with Smart Contract (Solidity) Development, Solana programs, smart contract testing, security audit program / smart contract and blockchain documentation.

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
[![Open Source](https://img.shields.io/badge/Open%20Source-Yes-brightgreen)](https://opensource.org/)

## ✨ Overview

This repository contains blockchain-specialized subagents that extend Claude Code's capabilities for blockchain development. Each subagent is an expert in a specific domain, automatically invoked based on context or explicitly called when needed. All agents are configured with Claude models optimized for task complexity to deliver optimal performance and cost-effectiveness.

## 🤖 Available Subagents

### 📚 [Blockchain Documentation Architect](blockchain-documentation-architect.md)
**Purpose**: Create comprehensive technical documentation for blockchain programs and smart contracts

**Capabilities**:
- Generate detailed documentation for Solana programs and EVM smart contracts
- Create Mermaid diagrams for data flows, PDA relationships, and system architecture
- Produce sequence diagrams for transaction flows and contract interactions
- Document program-derived addresses (PDAs), account structures, and instruction handlers
- Create visual representations of complex blockchain architectures

**Best for**: Program documentation, architectural diagrams, technical specifications, onboarding materials

### 🧪 [Solana QA Engineer](solana-qa-engineer.md) 
**Purpose**: Build comprehensive test suites for Solana programs

**Capabilities**:
- Write unit tests, integration tests, and end-to-end tests
- Expert knowledge of `litesvm`, `mollusksvm`, and `solana-program-test` frameworks
- Test PDA operations, Cross-Program Invocations (CPIs), and token operations
- Create test coverage for edge cases, error conditions, and security constraints
- Migrate tests between different testing frameworks

**Best for**: Test-driven development, quality assurance, regression testing, test framework migration

## 🚀 Getting Started

### Prerequisites
- [Claude Code](https://claude.ai/code) installed and configured
- Solana development environment (for Solana-specific agents)
- Rust and Anchor framework (recommended)

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/mads-finance/blockchain-agents.git
   cd blockchain-agents
   ```

2. **Configure Claude Code subagents**:
   Copy the subagent configuration files to your Claude Code workspace:
   ```bash
   # Copy subagent files to your Claude Code subagents directory
   cp *.md /path/to/your/claude-code/subagents/
   ```

3. **Verify installation**:
   The subagents will automatically become available in Claude Code and can be invoked contextually or explicitly.

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

### Automatic Context Detection
The subagents are automatically invoked when Claude Code detects relevant context:
- Creating or modifying Solana programs
- Working with blockchain documentation
- Writing or debugging tests for smart contracts

## 🏗️ Architecture

Each subagent is designed as a specialized expert with:

- **Domain Expertise**: Deep knowledge in specific blockchain development areas
- **Tool Integration**: Seamless integration with Claude Code's tool ecosystem  
- **Context Awareness**: Automatic activation based on development context
- **Extensibility**: Easy to modify and extend for specific project needs

## 🤝 Contributing

We welcome contributions from the blockchain development community!

### How to Contribute

1. **Fork the repository**
2. **Create a feature branch**: `git checkout -b feature/new-subagent`
3. **Make your changes**:
   - Add new subagents in the same markdown format
   - Update documentation and examples
   - Test your subagents thoroughly
4. **Submit a pull request**

### Contribution Guidelines

- Follow the existing subagent structure and formatting
- Include comprehensive documentation and examples
- Test all functionality before submitting
- Update the main README.md with new subagents

### Ideas for New Subagents

- **EVM Smart Contract Specialist**: For Ethereum/EVM development
- **Cross-Chain Bridge Expert**: For interoperability solutions  
- **DeFi Protocol Architect**: For decentralized finance applications
- **NFT Marketplace Developer**: For NFT-related functionality
- **Governance Protocol Designer**: For DAO and governance systems

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Built for the [Claude Code](https://claude.ai/code) ecosystem
- Inspired by the Solana and broader blockchain development communities
- Thanks to all contributors and users who help improve these tools

## 📞 Support

- **Issues**: Report bugs and request features via [GitHub Issues](https://github.com/mads-finance/blockchain-agents/issues)
- **Discussions**: Join conversations in [GitHub Discussions](https://github.com/mads-finance/blockchain-agents/discussions)
- **Documentation**: Additional docs and examples available in individual subagent files

---

**Happy Blockchain Building!** 🏗️⛓️
