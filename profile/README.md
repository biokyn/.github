<div align="center">

# BioKyn

**Bot protection that respects your users.**
Free, open source, self-hosted. No puzzles. No tracking. No third-party CAPTCHA.

[Website](https://biokyn.js.org) · [Documentation](https://github.com/biokyn/biokyn/tree/main/docs) · [npm](https://www.npmjs.com/org/biokyn) · [Discussions](https://github.com/biokyn/biokyn/discussions)

</div>

## What we build

BioKyn replaces "click all the traffic lights" with cryptographic proof. Visitors do a small amount of work in their browser, your server verifies it, and an anonymous single-use token is issued. Your data stays on your infrastructure.

| | |
|---|---|
| 🔐 **Private by design** | RFC 9497 VOPRF tokens, no cookies, no fingerprinting |
| ♿ **Accessible** | No pointer, vision or puzzle-solving required |
| ⚡ **Drop-in** | Express and Next.js adapters, reCAPTCHA/Turnstile-compatible `/siteverify` |
| 🏗️ **Production-ready** | Redis stores, fail-closed behavior, key rotation, signed releases |

## Get started

```bash
npm install @biokyn/server @biokyn/client
```

## Repositories

- [**biokyn**](https://github.com/biokyn/biokyn): the toolkit (server, client, protocol, core, shim)
- [**biokyn.github.io**](https://github.com/biokyn/biokyn.github.io): the project website

## Get involved

Read the [contributing guide](https://github.com/biokyn/biokyn/blob/main/CONTRIBUTING.md), pick up a `good first issue`, or start a conversation in [Discussions](https://github.com/biokyn/biokyn/discussions). Security reports go through [private advisories](https://github.com/biokyn/biokyn/security/advisories/new).

Licensed under [Apache-2.0](https://github.com/biokyn/biokyn/blob/main/LICENSE).
