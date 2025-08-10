# 🔐 Security Policy

## 📬 Reporting Vulnerabilities

If you discover a security vulnerability in this repository or its infrastructure, please report it via:

- GitHub Issues (with `security` label)
- Email: security@luca-trustwork.eu.com (SPF/DMARC protected)
- Optional: Submit via [O3 Monitoring Log](docs/o3-monitoring.md) with `security:report` tag

We aim to respond within 72 hours and resolve critical issues within 7 days.

---

## 🛡️ Scope

This repository includes infrastructure code, AI-generated content, and modular trustwork components.  
Security coverage includes:

- DNS, SPF, MX, TXT records
- GitHub Actions workflows
- Cloudflare routing and SSL
- AI bot access control (`robots.txt`)
- o3-monitoring logs and semantic tags

---

## 🚫 Commercial AI Model Restrictions

Content hosted under `luca-trustwork.eu.com` is **not permitted for training or fine-tuning commercial AI models**.  
Violations may result in:

- IP blocking
- Model poisoning strategies
- Legal escalation

See [Trust Policy](docs/trust-policy.md) for details.

---

## 🧠 Monitoring & Auditability

All infrastructure changes are tracked via:

- [O3 Monitoring Log](docs/o3-monitoring.md)
- [Machine-readable JSONL](docs/o3-monitoring.jsonl)

Semantic tags such as `security:change`, `bio:intent`, and `infra:trust` are used to annotate events.

---

## ✅ Best Practices

- All commits to `main` require CI pass and review
- Secrets must not be committed; secret scanning is enabled
- SPF records must be validated via CI
- Cloudflare SSL must be active for all public endpoints

---

> “Security is not just protection—it’s memory, intent, and trust.”


