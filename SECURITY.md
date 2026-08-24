# Security policy

Thank you for taking the time to report a problem responsibly.

## Reporting a vulnerability

Please **do not open a public issue** for a security problem.

Use **[GitHub's private vulnerability reporting](https://docs.github.com/code-security/security-advisories/guidance-on-reporting-and-writing-information-about-vulnerabilities/privately-reporting-a-security-vulnerability)**
on the affected repository — the *Security* tab, then *Report a vulnerability*. That opens a private
channel visible only to us, and it keeps the whole exchange in one place.

If the affected component is not one of our public repositories — the hosted platform at
`dashboard.infranest.app`, for example — please use private vulnerability reporting on
[`.github`](https://github.com/InfraNest-Infrastructure-Organized/.github/security/advisories/new) and we
will route it internally.

## What to include

- What you found, and where — a URL, an endpoint, a repository and version
- The steps to reproduce it, or a proof of concept
- What an attacker could do with it
- Anything we should avoid doing while investigating (a live customer account, a destructive action)

## What we will do

- **Acknowledge** your report within three working days
- Tell you whether we can reproduce it, and what we think the impact is
- Keep you updated while we fix it, and let you know when it ships
- Credit you when it is published, unless you would rather we did not

## Scope

In scope: the hosted platform, our public repositories, and the InfraNest agent once published.

Out of scope, because they are not ours to fix: vulnerabilities in the third-party providers InfraNest
connects to (registrars, DNS providers, clouds). Please report those to the provider directly.

Also out of scope: findings from automated scanners with no demonstrated impact, missing hardening
headers with no exploit path, and reports that require an attacker to already control the customer's
machine or account.

## Please do not

- Access, modify or delete data belonging to anyone but yourself
- Run denial-of-service or load tests against the platform
- Use social engineering against our staff or customers

Testing against your own organisation and your own data is welcome. If you need a test account to
investigate something safely, ask.
