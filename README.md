# Wave 🌊

Privacy-preserving payroll protocol for Web3. Built on Horizen.

## The Problem

Crypto payroll is completely transparent. Every salary is visible on-chain. Coworkers can see each other's earnings, competitors can identify top talent, and anyone can trace employee spending. This lack of privacy is a major barrier to crypto payroll adoption.

## The Solution

Wave enables companies to pay employees on-chain with complete privacy by default, while allowing employees to cryptographically prove income legitimacy when needed (mortgages, taxes, regulations).

**Key Innovation:** Privacy by default, compliance on demand. Employees control what they reveal and when.

## How It Works

1. **Employer Deposits** - Company deposits payroll into Wave's mixer pool with an attestation proving legitimate business purpose
2. **Private Transfer** - ZK-SNARKs transfer funds to employees without revealing who receives what
3. **Employee Choice** - Withdraw anonymously OR with attestation to prove income source

## Features

- 🔒 **Complete Privacy** - ZK-SNARKs hide all salary details and transaction links
- ✅ **Compliance Ready** - Cryptographic proofs for taxes, mortgages, and regulations
- ⚡ **Bulk Payroll** - Process 100+ employees in a single transaction
- 🛡️ **Selective Disclosure** - Employees control what information they reveal
- 🔐 **Attestation System** - EAS integration for verifiable fund legitimacy



## Architecture

```
Employer → Mixer Pool (ZK commitments + Merkle tree) → Employees
              ↓
         Attestations (EAS)
              ↓
    Anonymous OR Attested Withdrawals
```

## Use Cases

- **DAOs** - Private contributor payments
- **Crypto Companies** - Confidential employee salaries
- **Remote Work Platforms** - Privacy-preserving international payroll
- **Any Organization** - Paying employees without public salary disclosure

## Roadmap

- **Day 45:** Testnet deployment with core circuits
- **Day 90:** Full feature set + security review
- **Day 120:** Mainnet launch
- **Day 150:** First pilot users (250+ employees)

## Why Wave?

| Current Solutions | Wave |
|------------------|------|
| Traditional payroll: Fully transparent | ✅ Private by default |
| Mixers: Privacy but no compliance | ✅ Compliance on demand |
| Can't prove income legitimacy | ✅ Cryptographic income proofs |

## Getting Started

```bash
# Clone the repository
git clone https://github.com/OxMaaz/wave.git

# Install dependencies
cd wave
npm install

# Set up environment
cp .env.example .env

# Run tests
npm test
```

## Documentation

- [Technical Whitepaper](./docs/whitepaper.md)
- [Integration Guide](./docs/integration.md)
- [API Reference](./docs/api.md)

## Security

Wave is currently in development. Smart contracts and ZK circuits will undergo independent security audits before mainnet launch.

**Report vulnerabilities:** security@wave.protocol

## Contributing

We welcome contributions! Please see [CONTRIBUTING.md](./CONTRIBUTING.md) for guidelines.

## License

MIT License - see [LICENSE](./LICENSE) for details.

## Contact

- **Website:** wave.protocol (coming soon)
- **Twitter:** [@WaveProtocol](https://twitter.com/Wave__io)
- **Email:** maazweb3@gmail.com

## Acknowledgments

Built with support from the [Horizen Genesis Program](https://www.horizen.io/). Inspired by the privacy innovations of Tornado Cash and the compliance frameworks of traditional finance.

---

**⚠️ Disclaimer:** Wave is experimental software currently in development. Use at your own risk. Not audited for production use.
