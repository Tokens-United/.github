# Security Policy

Tokens United LLP (United Kingdom) builds and operates production systems that real businesses run on. Security isn't something we bolt on at the end — it's how we build. This page explains how to report a vulnerability and exactly what to expect from us in return.

## Reporting a vulnerability

**Please report security issues privately by email to [security@tokensunited.com](mailto:security@tokensunited.com).**

Do **not** open a public GitHub issue, pull request, or discussion for anything security-related. Public disclosure before a fix is in place puts users at risk.

To help us assess and resolve the issue quickly, please include:

- A clear description of the vulnerability and its potential impact.
- The affected platform, repository, endpoint, or component.
- Step-by-step instructions to reproduce it (proof-of-concept code, requests, or screenshots are welcome).
- Any relevant configuration, environment, or version details.
- Your name or handle if you'd like to be credited.

If you need to share sensitive details, mention it in your initial email and we'll arrange a secure channel.

## What to expect

- **Acknowledgement** — we will confirm receipt of your report within **3 business days**.
- **Assessment** — we'll triage the issue, validate it, and keep you informed of our findings and severity rating.
- **Resolution** — for confirmed vulnerabilities, our target is to remediate within **30 days**, prioritising by severity. Complex issues may take longer; we'll communicate timelines if so.
- **Credit** — with your permission, we're glad to acknowledge your contribution once the issue is resolved.

We ask that you give us a reasonable opportunity to investigate and remediate before any public disclosure.

## Scope

This policy covers Tokens United's web platforms and their APIs, along with the code in our repositories that powers them.

Our platforms are built with security as a baseline: session-based authentication (no JWTs), role-based access control (RBAC), audited sensitive actions, and secrets managed exclusively through `TU_`-prefixed environment variables. Reports that demonstrate a way to undermine these controls are especially valuable to us.

### Out of scope

The following are generally **not** in scope and will not be eligible for acknowledgement:

- Denial-of-service (DoS / DDoS) and volumetric or resource-exhaustion attacks.
- Social engineering of our team, partners, or users (including phishing).
- Physical attacks against offices, hardware, or personnel.
- Reports from automated scanners without a demonstrated, exploitable impact.
- Best-practice or hardening suggestions with no concrete security impact (e.g. missing headers with no exploit path).

## Safe harbour

We support good-faith security research. If you make a genuine, good-faith effort to comply with this policy, we will not pursue or support legal action against you for that research. To stay within safe harbour:

- Only test against accounts and data you own or are explicitly authorised to use.
- Avoid privacy violations, data destruction, service disruption, and any degradation of the experience for other users.
- Do not access, modify, or exfiltrate data that does not belong to you — stop and report as soon as you confirm a vulnerability.
- Keep details of the issue confidential until we've had a reasonable chance to remediate.

If you're unsure whether an action is permitted, ask us first at [security@tokensunited.com](mailto:security@tokensunited.com).

## Supported releases

We support the **latest production release** of each platform. Security fixes are applied to current production systems; older or superseded versions are not maintained.

---

Thank you for helping keep Tokens United and the businesses we serve secure.
