# DeFi Protocol Security Auditor

An AI-powered security auditing tool that analyzes DeFi protocols for potential vulnerabilities and exploits. This tool performs both individual smart contract analysis and system-wide interaction analysis to identify potential security risks.

## Features

- Automated smart contract vulnerability scanning
- System-wide interaction analysis
- Detection of common DeFi attack vectors
- Multi-threaded analysis for better performance
- Comprehensive JSON report generation
- Support for both Solidity and Vyper contracts

## Key Security Checks

1. Reentrancy vulnerabilities
2. Access control issues
3. Integer overflow/underflow
4. Flash loan attack vectors
5. Price manipulation vulnerabilities
6. Logic errors in financial calculations
7. Centralization risks
8. Cross-contract interaction risks
9. MEV opportunities
10. Oracle manipulation possibilities
11. Governance attack vectors

## Prerequisites

### Installing Git

#### macOS
Using Homebrew:

```bash
brew install git
```
Or download the installer from: https://git-scm.com/download/mac

#### Windows
Download and install from: https://git-scm.com/download/windows

#### Linux (Ubuntu/Debian)

```bash
sudo apt-get update
sudo apt-get install git
```

#### Linux (Fedora)

```bash
sudo dnf install git
```

Verify installation:

```bash
git --version
```

## Installation

```bash
pip install -r requirements.txt
```

## Configuration

Create a `.env` file in the project root:

```bash
echo "OPENAI_API_KEY=your-api-key-here" > .env
```

## Usage

```bash
python exploiter <repository_url> --output audit_report.json
```

### Arguments

- `repository_url`: URL of the GitHub repository to analyze
- `--output`: Output file for the audit report (default: audit_report.json)

## Output

The tool generates a detailed JSON report containing:
- Individual contract vulnerabilities
- System-wide vulnerabilities
- Severity levels
- Affected files
- Attack vectors
- Potential impact
- Recommendations for fixes

## Note

This tool is meant to assist security researchers and auditors. It should not be the only method of security analysis, but rather a part of a comprehensive security audit process.

## License

MIT # protocol-auditor
