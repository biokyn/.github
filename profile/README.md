# BioKyn

**Privacy-first bot mitigation. Built for developers. Designed for the open web.**

BioKyn is an open-source bot-mitigation toolkit designed to help web applications reduce automated form abuse without relying on traditional CAPTCHA challenges or mandatory third-party verification services.

By using cryptographically signed, short-lived, context-bound tokens, BioKyn provides developers with a lightweight way to verify form submissions and introduce friction against automated abuse while keeping the verification infrastructure under their control.

[**npm Package**](https://www.npmjs.com/package/@biokyn/core) · **[Source Code](https://github.com/biokyn/biokyn)** · **[Report an Issue](https://github.com/biokyn/biokyn/issues/new)**

---

## Our Mission

We believe security should not come at the expense of accessibility, privacy, or user experience.

BioKyn explores a developer-controlled approach to bot mitigation: reducing unnecessary verification friction for legitimate users while making automated abuse more difficult.

Our goal is to make practical, transparent security tools accessible to developers building applications of every size.

## Core Principles

| Principle | Our approach |
|---|---|
| **Privacy-conscious** | Designed to avoid dependence on third-party CAPTCHA verification services. |
| **Cryptographic integrity** | HMAC-SHA256 signed tokens bind verification to relevant request context. |
| **Developer-controlled** | Integrate verification into your own application infrastructure. |
| **Flexible storage** | Supports memory storage and integrations for SQLite and Redis. |
| **Open source** | Released under the Apache-2.0 license. |
| **Honest security** | Clearly documents limitations instead of claiming perfect bot prevention. |

## How It Works

1. **Issue** — The application generates a short-lived verification token.
2. **Bind** — The token is associated with relevant context, such as the form, origin, session, and requested action.
3. **Submit** — The client includes the token with the form submission.
4. **Verify** — The server validates the token and enforces the configured verification rules.
5. **Consume** — Single-use token handling helps prevent replay of previously accepted submissions.

## Get Started

Install the core package from npm:

```bash
npm install @biokyn/core
```

**Package:** [`@biokyn/core`](https://www.npmjs.com/package/@biokyn/core)  
**Current release:** `0.2.0`

See the package documentation for integration instructions, configuration options, storage adapters, and framework-specific examples.

## Security & Limitations

BioKyn is a bot-mitigation component, not a guarantee that every automated request can be detected or blocked.

A determined attacker may automate a real browser, obtain valid tokens, or bypass client-side controls. Effective protection depends on correct server-side verification, secure secret management, rate limiting, and deployment configuration.

We encourage security reviews, responsible vulnerability reports, and contributions that improve the project's reliability.

## Contributing

We welcome developers interested in web security, cryptography, backend engineering, testing, and open-source infrastructure.

Contributions can include:

- Bug reports and reproducible test cases
- Security reviews and responsible vulnerability disclosures
- Documentation improvements
- Framework integrations and storage adapters
- Automated tests and performance improvements

Please review the repository's contribution guidelines before submitting changes.

## License

BioKyn Core is distributed under the **Apache License 2.0**. Refer to the package repository for the applicable license and terms.

---

**BioKyn** — Practical bot mitigation, with transparency at its core.

