# Compliance & NIST CSF Mapping (Example)

This file documents a simple mapping of implemented controls to the NIST Cybersecurity Framework functions.

## Identify
- Inventory of cloud resources: Terraform + Cloud Asset Inventory
- IAM roles defined and limited privileges

## Protect
- Encryption in transit (HTTPS) and at rest (GCP-managed keys by default)
- Least-privilege IAM roles
- VPC / Firewall rules (if extended)

## Detect
- Cloud Logging enabled
- Security Command Center configured (recommended)

## Respond
- Alerts configured in Cloud Monitoring
- Playbooks for incident response (document and test)

## Recover
- Backups and export procedures for data (Cloud SQL export / storage)
