# Awesome Secrets Management

A curated directory of secrets managers, key vaults and secret-scanning tools.

## 📑 Table of Contents

- [Cloud Secret Stores & KMS (4)](#cloud-secret-stores--kms)
- [Developer .env Tools (1)](#developer-env-tools)
- [Kubernetes Secrets (2)](#kubernetes-secrets)
- [Open-Source Vaults (3)](#open-source-vaults)
- [Secret Scanning (4)](#secret-scanning)
- [Secrets Managers (7)](#secrets-managers)


## Cloud Secret Stores & KMS

- [AWS Secrets Manager](https://aws.amazon.com/secrets-manager) - AWS Secrets Manager is a managed service for storing and rotating database credentials, API keys, and other secrets in AWS. It integrates with IAM for fine-grained access control and supports automatic rotation for RDS. Pricing is per secret per month. ([Read more](/details/aws-secrets-manager.md)) `Paid` `Enterprise` `API` `Rotation` `HSM`
- [Azure Key Vault](https://azure.microsoft.com/en-us/services/key-vault) - Azure Key Vault is a cloud service for safeguarding cryptographic keys, certificates, and secrets used by Azure applications. It provides FIPS 140-2 Level 2 validated HSMs and integrates with Azure AD. Billing is based on operations and storage. ([Read more](/details/azure-key-vault.md)) `Paid` `Enterprise` `API` `HSM` `Certificates`
- [Fortanix Data Security Manager](https://www.fortanix.com/products/data-security-manager) - Fortanix Data Security Manager is a cloud-native HSM and key management service with confidential computing capabilities. It provides key lifecycle management, tokenization, and secrets management for hybrid clouds. Enterprise pricing with on-premises option. ([Read more](/details/fortanix-data-security-manager.md)) `Paid` `Enterprise` `API` `Self-Hosted` `HSM` `Confidential Computing`
- [Google Secret Manager](https://cloud.google.com/secret-manager) - Google Secret Manager is a fully managed service on Google Cloud for storing, accessing, and auditing secrets. It offers automatic replication, IAM integration, and audit logging. Charges apply per secret version and access operations. ([Read more](/details/google-secret-manager.md)) `Paid` `Enterprise` `API` `Replication` `Audit Logging`

## Developer .env Tools

- [Chamber](https://github.com/segmentio/chamber) - Chamber is an open-source CLI tool from Segment for managing secrets using AWS SSM Parameter Store and KMS. It provides a simple interface to write, read, and export secrets as environment variables. Licensed under MIT. ([Read more](/details/chamber.md)) `Open Source` `Free Plan` `Self-Hosted` `API` `AWS SSM` `KMS`

## Kubernetes Secrets

- [External Secrets Operator](https://external-secrets.io/) - External Secrets Operator is a Kubernetes operator that syncs secrets from external APIs (AWS, Azure, GCP, HashiCorp Vault) into Kubernetes Secrets. It supports multiple backends and is CNCF sandbox project. Licensed under Apache-2.0. ([Read more](/details/external-secrets-operator.md)) `Open Source` `Free Plan` `Self-Hosted` `API` `GitOps` `Multi-Backend`
- [Sealed Secrets](https://github.com/bitnami-labs/sealed-secrets) - Sealed Secrets is a Kubernetes controller and CLI for encrypting Kubernetes Secrets into SealedSecrets that are safe to store in Git. It uses a cluster-specific key pair and integrates with GitOps workflows. Maintained by Bitnami. ([Read more](/details/sealed-secrets.md)) `Open Source` `Free Plan` `Self-Hosted` `API` `GitOps` `Kubernetes`

## Open-Source Vaults

- [Keywhiz](https://github.com/square/keywhiz) - Keywhiz is an open-source secret management and distribution system from Square. It provides a server and CLI for storing and serving secrets with audit logging and ACLs. Designed for self-hosted deployment in microservice architectures. ([Read more](/details/keywhiz.md)) `Open Source` `Self-Hosted` `API` `Audit Logging` `Microservices`
- [Mozilla SOPS](https://github.com/mozilla/sops) - Mozilla SOPS (Secrets OPerationS) is an open-source editor for encrypted files using AWS KMS, GCP KMS, Azure Key Vault, or PGP. It integrates with Git and CI/CD to manage encrypted configuration files. Licensed under MPL-2.0. ([Read more](/details/mozilla-sops.md)) `Open Source` `Free Plan` `Self-Hosted` `API` `Encryption` `GitOps`
- [OpenBao](https://openbao.org/) - OpenBao is a community-driven fork of HashiCorp Vault maintaining the MPL license after Vault's license change. It provides the same dynamic secrets and encryption capabilities for self-hosted environments. Suitable for teams wanting a fully open-source Vault alternative. ([Read more](/details/openbao.md)) `Open Source` `Self-Hosted` `API` `Dynamic Secrets`

## Secret Scanning

- [detect-secrets](https://github.com/Yelp/detect-secrets) - detect-secrets is an open-source Python library and CLI from Yelp for identifying secrets in codebases. It provides a baseline file to track known secrets and integrates with pre-commit hooks. Licensed under MIT. ([Read more](/details/detect-secrets.md)) `Open Source` `Free Plan` `API` `Pre-commit` `Baseline`
- [GitGuardian](https://www.gitguardian.com/) - GitGuardian is a SaaS platform for detecting secrets and sensitive data in code repositories and CI/CD pipelines. It uses AI-powered detection and offers real-time alerts, remediation workflows, and compliance reporting. Free for individual developers, paid for teams. ([Read more](/details/gitguardian.md)) `Freemium` `Paid` `Enterprise` `API` `AI-Powered` `CI/CD`
- [Gitleaks](https://github.com/gitleaks/gitleaks) - Gitleaks is an open-source SAST tool for detecting hardcoded secrets in git repositories and files. It runs as a CLI, GitHub Action, or pre-commit hook with configurable rules. Free to use under MIT license. ([Read more](/details/gitleaks.md)) `Open Source` `Free Plan` `API` `Pre-commit` `GitHub Actions`
- [TruffleHog](https://trufflesecurity.com/) - TruffleHog is an open-source secret scanning tool that detects credentials in git history, files, and directories. It uses entropy checks and regex patterns with verification against live APIs. Offers a free CLI and paid enterprise features. ([Read more](/details/trufflehog.md)) `Open Source` `Free Plan` `API` `AI-Powered` `Verification` `Git History`

## Secrets Managers

- [Akeyless](https://www.akeyless.io/) - Akeyless is a SaaS secrets management platform with a free tier and enterprise features like dynamic secrets, certificate management, and zero-knowledge encryption. It supports hybrid deployment with a gateway for on-premises. Aimed at DevOps and security teams. ([Read more](/details/akeyless.md)) `Freemium` `Paid` `Enterprise` `API` `Dynamic Secrets` `Zero-Knowledge`
- [Bitwarden Secrets Manager](https://bitwarden.com/products/secrets-manager) - Bitwarden Secrets Manager is a commercial extension of the Bitwarden password manager for managing infrastructure secrets. It provides CLI, SDKs, and Kubernetes integration with a free tier for small teams. Built on zero-knowledge encryption. ([Read more](/details/bitwarden-secrets-manager.md)) `Freemium` `Paid` `Enterprise` `API` `Zero-Knowledge` `Kubernetes`
- [CyberArk Conjur](https://www.cyberark.com/products/conjur) - CyberArk Conjur is an enterprise secrets management solution for securing applications, containers, and CI/CD pipelines. It provides dynamic secrets, policy-as-code, and integrates with Kubernetes and cloud providers. Licensed per node with professional support. ([Read more](/details/cyberark-conjur.md)) `Paid` `Enterprise` `API` `Self-Hosted` `Dynamic Secrets` `Policy-as-Code`
- [Delinea Secret Server](https://delinea.com/products/secret-server) - Delinea Secret Server (formerly Thycotic) is a privileged access management vault for storing and rotating IT secrets. It offers on-premises and cloud deployment with session recording and compliance reporting. Targeted at enterprises managing privileged credentials. ([Read more](/details/delinea-secret-server.md)) `Paid` `Enterprise` `API` `Self-Hosted` `Privileged Access` `Session Recording`
- [Doppler](https://doppler.com/) - Doppler is a cloud-native secrets manager that syncs secrets across environments and CI/CD pipelines. It offers a free tier for individuals and paid plans for teams with audit logs and SSO. Integrates with major cloud providers and Kubernetes. ([Read more](/details/doppler.md)) `Freemium` `Paid` `Enterprise` `API` `CI/CD` `Kubernetes`
- [HashiCorp Vault](https://www.vaultproject.io/) - HashiCorp Vault is an open-source secrets management platform for dynamic secrets, encryption, and access control. It supports self-hosted deployment and offers an enterprise edition with advanced features. Widely used for infrastructure secrets across clouds. ([Read more](/details/hashicorp-vault.md)) `Open Source` `Self-Hosted` `Enterprise` `API` `Dynamic Secrets`
- [Infisical](https://infisical.com/) - Infisical is an open-source secrets management platform with a cloud-hosted free tier and self-hosted option. It manages API keys, certificates, and environment variables with Git-like versioning. Designed for developers and DevOps teams. ([Read more](/details/infisical.md)) `Open Source` `Self-Hosted` `Free Plan` `Freemium` `API` `GitOps`


## ™️ Legal

All product names, logos, and brands are the property of their respective owners. All company, product, and service names used in this repository, related repositories, and associated websites are for identification purposes only. The use of these names, logos, and brands does not imply endorsement, affiliation, or sponsorship.

This work may include content generated by artificial intelligence (AI). While efforts have been made to ensure the accuracy and reliability of the information, we make no representations or warranties of any kind, express or implied, about the completeness, accuracy, reliability, suitability, or availability of the information contained herein. Users are advised to independently verify the information before making decisions based on it.

We disclaim any responsibility for errors, omissions, or inaccuracies in the content, whether generated by humans, AI, or any other means. By using this work, you agree to use it at your own risk and acknowledge that the information provided may not always be current or accurate.

If you believe that your intellectual property rights or other legal rights have been infringed, please contact us immediately at legal@ever.co and we will take appropriate action.

## 🛡️ License

Shield: [![CC BY-SA 4.0][cc-by-sa-shield]][cc-by-sa]

This work is licensed under a

[Creative Commons Attribution-ShareAlike 4.0 International License][cc-by-sa].

[![CC BY-SA 4.0][cc-by-sa-image]][cc-by-sa]

[cc-by-sa]: http://creativecommons.org/licenses/by-sa/4.0/

[cc-by-sa-image]: https://licensebuttons.net/l/by-sa/4.0/88x31.png

[cc-by-sa-shield]: https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg