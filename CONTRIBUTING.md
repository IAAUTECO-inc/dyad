# Contributing to DYAD

Thank you for your interest in contributing to **DYAD**. As a project focused on **Sovereign AI** and **Critical Infrastructure**, we maintain high standards for code quality, security, and architectural integrity.

## Our Philosophy
DYAD is not just a tool; it is a framework for resilient, autonomous systems. We prioritize:
1. **Security by Design:** Every feature must minimize the attack surface.
2. **Deterministic Behavior:** We favor predictable outcomes over opaque "black-box" execution.
3. **Sovereignty:** We ensure the system remains agnostic and operable in air-gapped or restricted environments.

## Development Standards
To maintain a "Production-Critical" grade, all contributions must adhere to:
* **Strong Typing:** Mandatory use of Python type hints and strict Rust safety protocols.
* **Testing:** 100% coverage for logic-heavy modules. Integration tests must include failure-mode analysis.
* **Documentation:** Every public function and module must be documented using the Google Docstring format.

## Contribution Process
1. **Issue First:** Before submitting a Pull Request (PR), please open an issue to discuss the proposed change, especially for architectural modifications.
2. **Branching:** Use descriptive branch names (e.g., `feature/wasm-runtime` or `fix/telemetry-leak`).
3. **Signed Commits:** For traceability and legal compliance, all commits must be GPG-signed.
4. **DCO (Developer Certificate of Origin):** By contributing, you agree that your contribution is your original work and you have the right to license it under the project's Open Source license.

## Governance Model
DYAD follows a **Maintainer-Led Governance**:
* **Maintainers:** Expert architects responsible for the core roadmap and security audits.
* **Contributors:** Community members providing features, bug fixes, or documentation.
* **TSC (Technical Steering Committee):** For major architectural shifts (e.g., changing the core isolation layer), a consensus-based review is required.

---

### 2. SECURITY.md

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
