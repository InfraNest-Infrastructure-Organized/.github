# InfraNest

**Domains, DNS, cloud servers, certificates and uptime monitoring — in one place, across every provider.**

Most teams end up with domains at one registrar, DNS somewhere else, servers at a third provider,
certificates in a spreadsheet and monitoring in whatever was cheapest that year. InfraNest manages all of
it from one place, through the provider accounts you already have — there is nothing to migrate.

## What it manages

|  |  |
|---|---|
| **Domains** | Inventory across GoDaddy, IONOS, Namecheap, TransIP, Dynadot and Route 53 — registration, transfer, renewal, nameservers, contacts, transfer lock, WHOIS privacy and DNSSEC, each greyed out where the registrar or TLD genuinely cannot do it |
| **DNS** | Zones and records across Cloudflare, Hetzner, IONOS, TransIP, GoDaddy, Namecheap and Route 53, with live sync, drift detection, reusable templates and a security advisor |
| **Cloud** | Servers, volumes, firewalls, networks, load balancers and snapshots on Hetzner, TransIP and OVHcloud — power actions, rescue, rebuild, metrics and console |
| **Monitoring** | HTTP, keyword, redirect, port, SSL, DNS and ping checks from multiple regions, with agreement between probes before anything is called down, plus incidents, maintenance windows and public status pages |
| **Certificates** | One inventory from imports, provider stores and monitor observations — deduplicated by fingerprint, graded for health, auto-linked to domains |
| **Automations** | When *X* happens, if *Y*, do *Z* — a rule engine over the same event stream the webhooks use, with branches, waits and approval steps |

Organisations, custom roles, SSO and two-factor authentication, scoped API tokens, a complete audit trail,
cost reporting and import/export come with it. Everything the interface can do is available through the
REST API.

## Open source

InfraNest is a hosted service and the platform source is private. The parts that run on **your** machines
are published, so you can read exactly what they do before you install them.

First up is the **InfraNest agent** — an optional collector for the things a provider API cannot see:
memory, disk space per mount, load average and service health. It only ever *sends*. It accepts no
instructions, executes nothing on your machine, and opens no ports.

## Links

- **[infranest.app](https://infranest.app)** — the product
- **[support.infranest.app](https://support.infranest.app)** — help centre and documentation
