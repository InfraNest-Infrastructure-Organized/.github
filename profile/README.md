<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/InfraNest-Infrastructure-Organized/.github/main/profile/assets/infranest-logo-dark.svg">
    <img alt="InfraNest" src="https://raw.githubusercontent.com/InfraNest-Infrastructure-Organized/.github/main/profile/assets/infranest-logo-light.svg" width="320">
  </picture>
</p>

<p align="center">
  <strong>Domains, DNS, cloud servers, certificates and uptime monitoring —<br>
  in one place, across every provider.</strong>
</p>

<p align="center">
  <a href="https://app.infranest.io">Sign in</a> ·
  <a href="https://infranest.io">Product</a> ·
  <a href="https://infranest.io/docs/">Help center</a> ·
  <a href="https://developers.infranest.io">Developers</a> ·
  <a href="https://status.infranest.io">Status</a>
</p>

---

Most teams end up with domains at one registrar, DNS somewhere else, servers at a third provider,
certificates in a spreadsheet and monitoring in whatever was cheapest that year. InfraNest manages all of
it from one place, through the provider accounts you already have — there is nothing to migrate.

## What it manages

|  |  |
|---|---|
| **Domains** | Inventory across GoDaddy, IONOS, Namecheap, TransIP, Dynadot and Route 53 — registration, transfer, renewal, nameservers, contacts, transfer lock, WHOIS privacy and DNSSEC |
| **DNS** | Zones and records across Cloudflare, Hetzner, IONOS, TransIP, GoDaddy, Namecheap and Route 53, with live sync, drift detection, reusable templates and a security advisor |
| **Cloud** | Servers, volumes, firewalls, networks, load balancers and snapshots on Hetzner, TransIP and OVHcloud — power actions, rescue, rebuild, metrics and console |
| **Monitoring** | HTTP, keyword, redirect, port, SSL, DNS and ping checks from multiple regions, with agreement between probes before anything is called down, plus incidents, maintenance windows and public status pages |
| **Certificates** | One inventory from imports, provider stores and monitor observations — deduplicated by fingerprint, graded for health, auto-linked to domains |
| **Automations** | When *X* happens, if *Y*, do *Z* — a rule engine over the same event stream the webhooks use, with branches, waits and approval steps |

Organisations, custom roles, SSO and two-factor authentication, scoped API tokens, a complete audit trail,
cost reporting and import/export come with it. A REST API lets your own scripts, pipelines and AI tools do the
day-to-day work: DNS records, monitors, maintenance windows, incidents, status pages and more.

## Why one place

- **Nothing to migrate.** InfraNest drives the registrar, DNS and cloud accounts you already hold. Your
  domains stay where they are; you just stop logging into six control panels to find them.
- **Capabilities are honest.** Where a registrar or a TLD genuinely cannot do something, the button is
  greyed out and says why — rather than failing at the provider after you have clicked it.
- **Everything is accountable.** Every change is in the audit trail, including which API token made it, and
  alerts reach email, Slack, Teams, Discord, Telegram or PagerDuty.

## Build on InfraNest

- **[Developer documentation](https://developers.infranest.io)**: getting started, tokens and scopes, errors, and
  the full API reference.
- **A free sandbox** to try every write safely: sample data, test tokens, and nothing reaches a provider or the
  internet. See the [sandbox guide](https://developers.infranest.io/sandbox).
- **Safe by design**: scoped tokens that expire, per-token rate limits, dry runs for DNS changes, idempotency keys
  for retries, and a security email whenever a token is created.

## Open source

InfraNest is a hosted service and the platform source is private. The parts that run on **your** machines, and
everything you need to build on the API, are published, so you can read exactly what they do.

| Repository | What it is |
|---|---|
| [**infranest-agent**](https://github.com/InfraNest-Infrastructure-Organized/infranest-agent) | An optional collector for what a provider API cannot see: memory, disk space per mount, load average and service health. It only ever *sends*: it accepts no instructions, executes nothing, and opens no ports. |
| [**infranest-examples**](https://github.com/InfraNest-Infrastructure-Organized/infranest-examples) | Ready-to-run scripts for the API in shell, Python, JavaScript and PowerShell: dynamic DNS, Let's Encrypt DNS-01, maintenance windows from CI, monitors per deploy, the audit log to a SIEM. |
| [**infranest-action**](https://github.com/InfraNest-Infrastructure-Organized/infranest-action) | InfraNest in a GitHub Actions workflow: silence alerts while you deploy, pause monitors, reset your sandbox. |
| [**infranest-openapi**](https://github.com/InfraNest-Infrastructure-Organized/infranest-openapi) | The public API described in OpenAPI 3, updated daily, with a release for every change. Generate a client or give it to your AI tools. |

The examples and the action are checked against the published API every week and on every change, so what you
copy keeps working.

## Security

Found a vulnerability? Please report it privately — see [SECURITY.md](../SECURITY.md).
