# Contributing to xMesh / NovaNet / QNET

This repository focuses on the **practical implementation** of decentralized mesh networking: Docker orchestration, Yggdrasil configurations, deployment scripts, troubleshooting, hardware support (Tenda Nova), privacy hardening, and integration with the broader ecosystem (Xanadu protocol core + Nexus orchestration).

## Code of Conduct

Collaborative, respectful, and focused on real-world deployability and privacy. Contributions from system administrators, Docker enthusiasts, networking tinkerers, privacy advocates, and hardware hackers are especially valued.

## How to Contribute

### Issues
Use labels such as:
- `docker`
- `yggdrasil`
- `config`
- `troubleshooting`
- `privacy`
- `tenda-nova`
- `integration-xanadu`
- `integration-nexus`
- `documentation`

Provide: OS/Docker version, exact commands run, logs, network topology description, and what you expected vs. observed.

### Pull Requests
1. Create a feature branch from `main`.
2. Keep changes focused and atomic.
3. Update or add documentation alongside code/config changes.
4. Test Docker setups locally when possible.
5. Use clear commit messages (e.g., "feat(docker): add multi-node testnet compose with chaos testing").

### Development & Testing
- Primary environment: Linux + Docker
- Use `docker compose` for reproducible multi-node meshes
- Yggdrasil nodes can be run in containers or natively
- For hardware: Tenda Nova or similar OpenWrt-based devices
- Always prioritize security and privacy defaults

### Contribution Areas

**Docker & Orchestration**
- Improved compose files for different scales (single node, testnet, production simulation)
- Healthchecks, logging, and monitoring integration
- Volume and network configuration best practices

**Yggdrasil & Core Networking**
- Configuration templates for different peering strategies
- Scripts for automated peering, status monitoring, and restarts
- NAT traversal and firewall helper scripts

**Privacy & Security**
- Tor/I2P transport configuration examples
- Hardened defaults and security checklists
- Secrets management (never commit keys or .env files)

**Hardware & Embedded**
- Tenda Nova and similar device setup guides
- Cross-compilation or lightweight deployment notes
- Monitoring hooks for resource-constrained nodes

**Integration**
- Examples showing how xMesh/NovaNet/QNET nodes work with Xanadu messaging/broadcast layer
- Hooks and adapters for Nexus orchestration and monitoring
- Future QNET blockchain coordination examples

**Documentation & Troubleshooting**
- Step-by-step guides for common issues (peering failures, Docker networking problems, restart loops)
- FAQ and decision trees
- Video or diagram contributions welcome

## Style Guidelines
- Configuration files should be well-commented
- Scripts should be idempotent and safe to re-run
- Documentation must include prerequisites, exact commands, and expected output
- Edge cases (intermittent connectivity, partial network partitions, resource limits) should be addressed

## Recognition
Contributors will be credited in releases and documentation. Significant work may lead to deeper collaboration opportunities within the Esslinger & Co. ecosystem.

Questions? Open an issue or reach out on X (@SirLancelotEsq).

Thank you for helping make decentralized mesh networking practical and accessible.