```markdown
# Security Policy

## Our Commitment
As a cybersecurity-centric project, the security of **DYAD** is our highest priority. We recognize the unique risks associated with LLM-driven system orchestration (e.g., prompt injection, unauthorized code execution).

## Supported Versions
Only the latest stable version of DYAD receives security updates. We recommend all institutional users stay aligned with the `main` branch or official tagged releases.

## Reporting a Vulnerability
**Do not open a public GitHub issue for security vulnerabilities.**

To report a sensitive bug, please follow this protocol:
1. Send an encrypted email to [security-email@your-domain.org] (or use the GitHub Private Vulnerability Reporting feature).
2. Include a detailed description of the vulnerability, a Proof of Concept (PoC), and the potential impact on sovereign infrastructures.
3. Our security team will acknowledge receipt within **24 hours**.

## Disclosure Policy
We follow a **90-day coordinated disclosure policy**. We will work with you to fix the vulnerability and will credit you for the discovery upon the release of the patch, unless you prefer to remain anonymous.

## Prohibited Contributions
Any contribution that introduces:
* Hardcoded credentials
* Unsafe deserialization
* Bypassing of the WASM/Sandbox isolation layer
...will be rejected immediately and may lead to a permanent ban from the organization.
