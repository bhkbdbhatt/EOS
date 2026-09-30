# Contributing Guidelines

Thank you for your interest in contributing to the **Enterprise Open Source Architecture Matrix & Evaluation Suite**. 

This project aims to deliver objective, field-tested, and opinionated architectural evaluations for self-hosted enterprise open-source software. We welcome contributions from Enterprise Architects, SREs, Security Engineers, and DevOps Practitioners.

---

## 📐 Core Evaluation Philosophy

Before submitting a change, please align your contribution with our foundational principles:

1. **Opinionated over Neutral:** Avoid "it depends" responses. Every tool assessment must state a default enterprise verdict and clear conditions under which that recommendation changes.
2. **Production-First Realism:** Assessments must reflect real-world operational overhead—focusing on failure modes, day-two maintenance burden, database migration complexity, and SRE paging risk.
3. **Total Cost of Ownership (TCO):** Licensing is only one component of cost. Compute resources, storage footprints, and FTE operational maintenance hours must always be factored into evaluations.
4. **License & Supply Chain Transparency:** Clearly highlight license shifts (e.g., AGPLv3, BSL, SSPL) and supply-chain risks (SBOM support, CIS benchmarks).

---

## 🛠 Ways to Contribute

We welcome contributions in the following areas:

*   **Tool Profile Updates:** Updating existing tool assessments based on new software releases, architectural changes, or license updates.
*   **New Tool Proposals:** Recommending new production-grade open-source tools for inclusion in future matrix iterations.
*   **IaC Blueprint Improvements:** Enhancing Helm charts, Kustomize overlays, or Terraform modules provided in enterprise bundles.
*   **Bug Fixes & UX Enhancements:** Improving the interactive web interface, data parsing, filtering logic, or accessibility.

---

## 📋 Tool Assessment Submission Format

When submitting a new tool assessment or revising an existing one, you **must** follow this structure:

```markdown
### [Tool Name] ([License])

- **Deployment & Architecture:** [Monolithic/Microservice topology, compute/RAM footprint, state dependencies, background execution engines]
- **Core Capabilities & Limits:** [Primary functional strengths, key scaling limitations, missing enterprise features]
- **TCO & Operational Overhead:** [Human-hour maintenance burden, database migration friction, upgrade complexity]
- **Security & Compliance:** [License risks, SAML/OIDC availability, RBAC granularity, audit logging, SBOM support]
- **Interoperability & API:** [REST/GraphQL capabilities, SDK support, webhooks, third-party integrations]
- **Architecture Diagram & Data Flow:**
  ```text
  [Component A] ---> [Component B] ---> [Data Store]

```

* **Enterprise Verdict:** [RECOMMENDED / RECOMMENDED WITH CAUTION / NOT RECOMMENDED] + [Single-sentence contextual directive]

```

---

## 🔀 Pull Request Process

1. **Fork the Repository:** Create your own fork of the project and branch off from `main`.
2. **Create a Feature Branch:**
   ```bash
   git checkout -b feature/update-valkey-eval
   # OR
   git checkout -b fix/matrix-filter-bug

```

3. **Commit Your Changes:** Write concise, descriptive commit messages following Conventional Commits format:
* `feat: add evaluation for new observability tool`
* `fix: correct license metadata for Valkey`
* `docs: update deployment guidelines in README`


4. **Test Locally:** If modifying the web application, open `index.html` in a clean browser environment to verify rendering, matrix filtering, stack configurator logic, and responsive layouts across viewports.
5. **Submit a Pull Request:**
* Provide a clear description of the changes and rationale.
* Reference any relevant open issues.
* Ensure your PR passes all automated status checks.



---

## ⚖️ Code of Conduct

We are committed to providing a welcoming, collaborative, and professional environment for all contributors.

* Treat all community members with respect and professionalism.
* Focus feedback on architectural claims, objective evidence, and technical data.
* Avoid vendor-centric promotional hype or unsupported marketing assertions.

---

## 📄 License

By contributing to this repository, you agree that your contributions will be licensed under the project's [MIT License](https://www.google.com/search?q=LICENSE).

```

```
