[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![License: Apache 2.0](https://img.shields.io/badge/License-Apache_2.0-green.svg)](https://www.apache.org/licenses/LICENSE-2.0)
[![CI Status](https://img.shields.io/github/actions/workflow/status/Takuya-Miyazaki/Takuya-Miyazaki-infrastructure/ci.yml?branch=main)](https://github.com/Takuya-Miyazaki/Takuya-Miyazaki-infrastructure/actions)



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
