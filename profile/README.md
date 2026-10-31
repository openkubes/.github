<a href="https://openkubes.org/"><img src="https://raw.githubusercontent.com/openkubes/openkubes/main/docs/openkubes-logo.png" alt="OpenKubes logo" width="240"></a>

# OpenKubes — Sovereign Platform Engineering

**Contracts First. Evidence Driven. Human Controlled.**

OpenKubes is an open-source framework for building sovereign Kubernetes platform distributions.
It defines platform contracts, architectural principles and conformance rules,
while implementations can change to suit different environments.

**OpenKubes Platform (OKP)** is the official reference distribution and conforms
to the OpenKubes contracts. Deploy OKP as provided, adapt it, or use OpenKubes to
build your own distribution. Conformance is scoped to a contract version and a
profile or applicability declaration; it is not a blanket certification.

> OpenKubes owns the contracts, not the components.

[Website](https://openkubes.org/) · [Getting Started](https://openkubes.org/getting-started/) · [Console Documentation](https://openkubes.org/console/)

## Why OpenKubes

- **Contracts:** Define the guarantees a capability must honor before choosing its components.
- **Evidence:** Use contract tests and recorded observations to check those guarantees.
- **Sovereignty:** Choose implementation profiles and provider values for the infrastructure you control.
- **Human control:** AI can analyze and propose; humans approve architectural decisions and merge changes.

The engineering chain connects **Capability → Contract → Implementation Profile →
Provider Values → Contract Tests**. The [platform engineering method](https://github.com/openkubes/openkubes/blob/main/docs/platform-engineering-method.md)
explains the boundaries behind it.

## Explore the OpenKubes ecosystem

### Framework & Architecture

| Repository | Purpose |
| --- | --- |
| [openkubes](https://github.com/openkubes/openkubes) | Framework contracts, architecture decisions, conformance rules and the shared integration layer. |
| [.github](https://github.com/openkubes/.github) | This organization profile and its maintenance notes. |

### Console & Developer Experience

| Repository | Purpose |
| --- | --- |
| [ok-console](https://github.com/openkubes/ok-console) | Platform Console prototype with deterministic fixture data and a read-only backend integration path. |
| [ok-local](https://github.com/openkubes/ok-local) | Local learning and development environment using K3s, Multipass and KubeVirt on macOS. |

### Cluster Lifecycle & Infrastructure

| Repository | Purpose |
| --- | --- |
| [ok-cluster](https://github.com/openkubes/ok-cluster) | Cluster lifecycle engine with Cluster API integration and a bounded `ok` CLI MVP. |
| [ok-linux](https://github.com/openkubes/ok-linux) | Curated Kubernetes host-OS profiles: Talos by default, with a constrained Flatcar/KubeVirt profile. |
| [ok-rke2](https://github.com/openkubes/ok-rke2) | Ansible role for deploying RKE2 clusters on Hetzner bare-metal servers. |
| [oke](https://github.com/openkubes/oke) | OpenKubes Kubernetes Engine, with server/agent installation and node-join workflows. |

### Platform Capabilities

| Repository | Purpose |
| --- | --- |
| [ok-storage](https://github.com/openkubes/ok-storage) | Persistent storage contracts, stable storage-class interfaces and implementation profiles. |
| [ok-observability](https://github.com/openkubes/ok-observability) | Observability contracts, per-cluster reference implementation assets, profiles and contract tests. |

### Community & Learning

| Repository | Purpose |
| --- | --- |
| [oki](https://github.com/openkubes/oki) | Illustrated stories and technical guides that introduce the OpenKubes universe. |

### Additional Projects — Open-RMF

These repositories are forks of Open-RMF projects, separate from the framework's core capability repositories.

| Repository | Purpose |
| --- | --- |
| [rmf-web](https://github.com/openkubes/rmf-web) | Open-RMF web interfaces, including an API server, API client and dashboard framework. |
| [rmf_deployment_template](https://github.com/openkubes/rmf_deployment_template) | Open-RMF deployment template adapted for RKE2, with Traefik ingress, cert-manager TLS and monitoring integration. |

## Getting Started

1. **Understand the framework:** Visit [Getting Started](https://openkubes.org/getting-started/) and explore the [framework repository](https://github.com/openkubes/openkubes).
2. **Evaluate the Console:** Follow the [Console documentation](https://openkubes.org/console/) for its local evaluation path. The Console is a prototype; its default fixture mode is not live cluster state.
3. **Learn locally:** Follow the prerequisites and tutorials in [ok-local](https://github.com/openkubes/ok-local) for the Multipass/K3s environment.
4. **Explore cluster lifecycle tooling:** Read [ok-cluster](https://github.com/openkubes/ok-cluster) for supported workflows and current execution gates. Its CLI MVP is not a general one-command cluster installer.

Maturity and supported environments vary by repository and profile. Check the
relevant README and validation guidance before deploying; prototype screens and
roadmap items are not production guarantees.

## Architecture and Documentation

- [Architecture overview](https://openkubes.org/architecture/)
- [Architecture Decision Records](https://github.com/openkubes/openkubes/tree/main/architecture/decisions)
- [Naming and terminology](https://github.com/openkubes/openkubes/blob/main/NAMING.md)
- [Contracts, not components](https://github.com/openkubes/openkubes/blob/main/architecture/decisions/ADR-Platform-001-contracts-not-components.md)

## Community and Contributions

Newcomers, platform engineers, documentation contributors and open-source
maintainers are welcome. Ask questions, report reproducible issues, improve a
tutorial, or propose a focused change in the repository that owns the capability.

Start with the [community page](https://openkubes.org/community/) and the
[contribution guide](https://github.com/openkubes/openkubes/blob/main/CONTRIBUTING.md),
then follow the target repository's README and contribution instructions.
Architectural proposals should reference the relevant contracts and ADRs.

[Explore all repositories](https://github.com/openkubes) · [Framework issues](https://github.com/openkubes/openkubes/issues)
