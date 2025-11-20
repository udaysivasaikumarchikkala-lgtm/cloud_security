# Secure Cloud Café

**Secure Cloud Café** is a hands-on, real-world project template that demonstrates building,
deploying, and operating a secure cloud-hosted web application using Google Cloud Platform,
Terraform (IaC), Docker, GitHub Actions (CI/CD), and DevSecOps tools (Trivy).

## What's included
- `src/` : Simple Flask backend + Dockerfile
- `infra/` : Terraform configuration for GCP Cloud Run + Storage bucket
- `.github/workflows/` : GitHub Actions workflows (build/deploy + Trivy scan)
- `compliance.md` : NIST CSF mapping and compliance notes
- `security/` : placeholder for security policies

## Quick start (high-level)
1. Create a Google Cloud project and enable required APIs (Cloud Run, Cloud Build, IAM, Cloud Storage).
2. Create a service account and add its JSON key as GitHub secret `GCP_SA_KEY`.
3. Add `GCP_PROJECT` as a GitHub secret with your project ID.
4. Push this repository to GitHub.
5. On `git push` to `main`, GitHub Actions will build the container, run Trivy scan, and deploy via Terraform.

> See `infra/` and `.github/workflows/` for details and customize as needed.

## Project ideas / extensions
- Add Cloud SQL and use SQL-based persistence
- Add authentication (OAuth2 / Firebase Auth)
- Add automated compliance reporting
- Integrate monitoring dashboards (Prometheus/Grafana)

