<div align="center">

# KTB Group · Self-Hosted Services

**A homelab and self-hosted infrastructure organization.**

Everything here runs on owned hardware and cloud infra — provisioned as code,
deployed as containers, and documented as it grows.

</div>

---

## Quick Links

**Queries**
- **[infra.* Repos](https://github.com/orgs/ktbgroup-self-hosted/repositories?q=infra)**
- **[stack.* Repos](https://github.com/orgs/ktbgroup-self-hosted/repositories?q=stack.)**

**Important Repos**
- **[documentation](https://github.com/ktbgroup-self-hosted/documentation)** — architecture, best practices, and the rules of the road
- **[template.stack](https://github.com/ktbgroup-self-hosted/template.stack)** — spin up a new service stack the right way
- **[home-assistant-blueprints](https://github.com/ktbgroup-self-hosted/home-assistant-blueprints)** — automation blueprints for Home Assistant

## How it's organized

Repositories follow a flat, prefix-based naming convention so the whole estate reads at a glance:

| Prefix | Purpose | Examples |
| --- | --- | --- |
| `infra.*` | Infrastructure-as-code — provision the machines and the cloud | `infra.terraform`, `infra.pyinfra`, `infra.desktops` |
| `stack.*` | Docker Compose stacks — the services that actually run | `stack.network`, `stack.apps`, `stack.biz-ops` |
| `template.*` | Reusable starting points | `template.stack` |

## The toolchain

- **Cloud** — [Hetzner](https://www.hetzner.com/) servers, firewalls, networks & DNS, managed with **Terraform**
- **Provisioning** — server & desktop config via **pyinfra**
- **Orchestration** — **Docker Compose** stacks, deployed through a central orchestrator
- **Networking** — reverse proxy + wildcard TLS fronting every service
- **Secrets** — centralized secret management, never in the repo

---

<div align="center">
<sub>Most repos here are private. The public ones are the ones worth sharing.</sub>
</div>
