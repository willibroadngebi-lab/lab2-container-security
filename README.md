# Lab 2: Container Security

## Overview
This lab demonstrates container security using Docker, Trivy, SBOM, and OPA Gatekeeper.

## Vulnerable Container
- Built using Python 3.8
- Installed Flask 1.0.0
- Scanned with Trivy
- Found multiple HIGH and CRITICAL vulnerabilities

## Hardened Container
- Updated to Python 3.12-slim-bookworm
- Upgraded Flask to 3.0.0
- Added non-root user
- Reduced image size using --no-cache-dir
- Added healthcheck
- Re-scanned with fewer vulnerabilities

## SBOM
- Generated using Trivy in CycloneDX format
- Lists all components in the container
- Useful for security and compliance

## Gatekeeper Policies
- Created a policy requiring labels on pods
- Tested deny and allow scenarios
- Verified policy enforcement

## Tools Used
- Docker
- Trivy
- Kubernetes
- OPA Gatekeeper

## Screenshots
See screenshots/ folder for:
- Trivy scans (before and after)
- Gatekeeper deny and allow results

## Conclusion
This lab shows how container security can be improved by reducing vulnerabilities, enforcing policies, and tracking dependencies.




