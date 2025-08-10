# lucia-group.uk.com DNS & SPF Infrastructure

This repository documents the modular DNS and SPF configuration for `lucia-group.uk.com`, designed to support operational sovereignty, auditability, and scalable email infrastructure for responsible AI deployment.

## Overview

This configuration enables:

- Modular sender authorization via SPF
- Separation of display-only and operational domains
- Version-controlled DNS records for auditability
- Future integration with CI/CD and DNS APIs (e.g., AWS Route53)
- License-compliant infrastructure for commercial and open use

## SPF Configuration

### Primary SPF Record (`lucia-group.uk.com`)

```txt
v=spf1 include:_spf.lucia-group.uk.com -all
