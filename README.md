KODOSKOP Cloud Developer Kit

Open-source AI development toolkit for software analysis, reverse engineering research, and legacy system modernization.

KODOSKOP Cloud Developer Kit provides agent skills, MCP integration tools, and automated installation scripts for working with KODOSKOP Cloud through OpenAI Codex and MiniMax Code.

The toolkit is designed to support the development and integration of KODOSKOP Cloud, a browser-based platform for authorized static software analysis, evidence collection, architecture reconstruction, and technical documentation.

## Features

- **AI Agent Integration** — Skills for OpenAI Codex and MiniMax Code.
- **Model Context Protocol (MCP)** — Integration bridge for connecting AI coding agents to KODOSKOP Cloud APIs.
- **Static Software Analysis** — Workflows designed around Ghidra and REA.
- **Architecture Reconstruction** — Evidence-based documentation of legacy software systems.
- **AI Gateway Development** — Structured analysis, tool calling, token budgets, and model integration.
- **Security Review** — Guidance for tenant isolation, access control, and secure processing.
- **Automated Installation** — Python-based skill installation and environment configuration.

## Included Agent Skills

| Skill | Description |
|---|---|
| `kodoskop-architecture` | SaaS architecture, APIs, database design, and RBAC |
| `kodoskop-static-analysis` | Static analysis using REA and Ghidra |
| `kodoskop-ai-gateway` | AI integration, evidence validation, and cost controls |
| `kodoskop-security-review` | Security architecture and isolation testing |
| `kodoskop-release` | Deployment, Docker, CI/CD, and release procedures |
| `kodoskop-investigation` | Software investigation through MCP tools |

## Installation

Clone the repository:

```bash
git clone https://github.com/eukundrotas/kodoskop-cloud-developer-kit.git
cd kodoskop-cloud-developer-kit
```

Install agent skills:

```bash
python3 scripts/install.py --target both --project /path/to/your/project
```

For Windows:

```powershell
py scripts/install.py --target both --project C:\Projects\kodoskop
```

For MCP configuration and platform-specific setup, see `docs/INSTALL.md`.

## Technology Stack

- **Frontend:** Next.js, React, TypeScript
- **Backend:** NestJS, PostgreSQL, Redis
- **Storage:** S3 / MinIO
- **Software Analysis:** REA, Ghidra
- **AI Integration:** OpenAI Responses API
- **Agent Connectivity:** Model Context Protocol
- **Infrastructure:** Docker Compose, Linux
- **Monitoring:** OpenTelemetry

These technologies describe the planned KODOSKOP Cloud architecture, not a fully implemented platform included in this repository.

## Project Status

**Version:** 0.1.0 — Early Development

This repository contains developer integration tools, agent skills, and project documentation. It does not include a production-ready KODOSKOP Cloud SaaS deployment.

The MCP bridge requires a compatible KODOSKOP API server. Live API compatibility and production security must be validated before deployment.

## Roadmap

1. Architecture and security foundations
2. Core web platform and project management
3. Static software analysis integration
4. AI-assisted evidence interpretation
5. Visualization and technical reporting
6. Security hardening and self-hosted deployment

See `ROADMAP.md` for additional details.

## Security and Responsible Use

KODOSKOP is intended for authorized software research, interoperability studies, and legacy application modernization.

The initial architecture uses static analysis only. Execution of uploaded binaries, bypassing software licensing, and unauthorized access are not supported product objectives.

Report security vulnerabilities according to `SECURITY.md`.

## Contributing

Community contributions, documentation improvements, integration testing, and bug reports are welcome.

Please read `CONTRIBUTING.md` before submitting a pull request.

## License

Distributed under the **MIT License**. See [LICENSE](LICENSE).

## Maintainer

GitHub: [@eukundrotas](https://github.com/eukundrotas)

---

**KODOSKOP Cloud — Understand software. Preserve evidence. Rebuild with confidence.**
