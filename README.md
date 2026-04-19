# HIPAA Cloud Governance Framework

**A Cloud TPM's compliance-as-code framework for building and maintaining HIPAA-compliant AWS infrastructure — covering encryption, IAM, audit automation, and continuous monitoring.**

![AWS](https://img.shields.io/badge/AWS-Cloud-orange?style=flat-square&logo=amazonaws)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=flat-square)
![Role](https://img.shields.io/badge/Role-Cloud%20TPM-blue?style=flat-square)

---

## Project Overview

This framework documents a comprehensive HIPAA compliance program for AWS cloud infrastructure. It reflects real-world TPM leadership in translating regulatory requirements into engineering controls, automating audit evidence collection, and maintaining continuous compliance across a regulated healthcare environment.

**Business Context:** The organization was expanding its cloud footprint in a HIPAA-regulated environment with manual compliance processes that consumed 200+ engineering hours per audit cycle. This framework automated 85% of compliance evidence collection, reduced audit preparation time by 70%, and achieved zero findings across two consecutive external audits.

---

## Repository Structure

hipaa-cloud-governance-framework/
|-- audit-automation/   # Automated compliance scanning, evidence collection, and reporting
|-- controls/           # HIPAA control mappings, policy-as-code definitions
|-- encryption/         # Encryption-at-rest and in-transit configurations, KMS policies
|-- iam/                # Role-based access controls, least-privilege policies, MFA enforcement
|-- monitoring/         # CloudTrail logging, GuardDuty configs, compliance dashboards
|-- README.md

---

## Compliance Framework

| HIPAA Safeguard | AWS Implementation | Status |
|----------------|-------------------|--------|
| Access Controls (§164.312(a)) | IAM policies, MFA, role-based access, session management | **Implemented** |
| Audit Controls (§164.312(b)) | CloudTrail, AWS Config Rules, automated evidence collection | **Implemented** |
| Integrity Controls (§164.312(c)) | Checksums, versioning, tamper-evident logging | **Implemented** |
| Transmission Security (§164.312(e)) | TLS 1.2+, VPN tunnels, encrypted API endpoints | **Implemented** |
| Encryption (§164.312(a)(2)(iv)) | KMS-managed keys, EBS/S3/RDS encryption at rest | **Implemented** |

---

## Key Results

| Metric | Before | After | Impact |
|--------|--------|-------|--------|
| Audit Prep Time | 6 weeks manual | under 2 weeks automated | **-70% reduction** |
| Compliance Evidence Collection | Manual/quarterly | Automated/continuous | **Real-time visibility** |
| External Audit Findings | 3-5 per cycle | 0 findings | **Clean audit record** |
| Engineering Hours per Audit | 200+ hours | under 60 hours | **140+ hours reclaimed** |
| Policy Drift Detection | Monthly manual review | Real-time automated | **Instant remediation** |

---

## Domain Breakdown

### `/controls` — HIPAA Control Mappings
- HIPAA Security Rule to AWS service control mapping matrix
- Policy-as-code definitions using AWS Config Rules
- Control inheritance model for shared responsibility documentation
- Gap analysis templates for new service onboarding

### `/encryption` — Data Protection
- KMS key policies and rotation schedules
- EBS, S3, and RDS encryption-at-rest configurations
- TLS certificate management and enforcement policies
- PHI data classification and handling procedures

### `/iam` — Identity & Access Management
- Role-based access control (RBAC) framework for healthcare teams
- Least-privilege policy templates for clinical and engineering roles
- MFA enforcement and conditional access policies
- Service account governance and credential rotation automation

### `/audit-automation` — Compliance Automation
- AWS Config Rules for continuous compliance monitoring
- Automated evidence collection scripts for audit packages
- Compliance dashboard configurations for executive reporting
- Remediation runbooks for common policy violations

### `/monitoring` — Security Monitoring & Logging
- CloudTrail configuration for all-region API logging
- GuardDuty threat detection and alerting setup
- VPC Flow Log analysis for network anomaly detection
- SIEM integration patterns for centralized security monitoring

---

## Tools & Services

| Category | Tools |
|----------|-------|
| **AWS Services** | IAM, KMS, CloudTrail, AWS Config, GuardDuty, S3, RDS, EBS |
| **Compliance** | AWS Config Rules, Security Hub, AWS Audit Manager |
| **Monitoring** | CloudWatch, GuardDuty, VPC Flow Logs, CloudTrail |
| **Automation** | Lambda, EventBridge, SNS, Systems Manager |
| **Program Management** | Jira, Confluence, ServiceNow |

---

## TPM Lens — Program Management Perspective

This project demonstrates core Cloud TPM competencies:

- **Regulatory Translation:** Converted HIPAA Security Rule requirements into actionable engineering controls with clear acceptance criteria
- **Cross-Functional Coordination:** Aligned Security, Engineering, Legal, and Compliance teams on shared control ownership and remediation SLAs
- **Audit Readiness:** Built continuous compliance pipeline that eliminated last-minute audit scrambles and produced audit-ready evidence packages on demand
- **Risk Quantification:** Developed compliance risk scoring model that prioritized remediation efforts by business impact and regulatory exposure
- **Process Automation:** Reduced manual compliance work by 85% through policy-as-code, automated scanning, and self-healing remediation workflows

---

## Related Projects

| Project | Description |
|---------|-------------|
| [Cloud Migration Architecture](https://github.com/Ewuack/cloud-migration-architecture) | On-prem to AWS migration program |
| [AWS Cost Optimization Playbook](https://github.com/Ewuack/aws-cost-optimization-playbook) | Strategic cost reduction across AWS infrastructure |
| [Cloud Incident Response Simulation](https://github.com/Ewuack/cloud-incident-response-simulation) | Security incident detection and response |
| [Cloud SDLC Pipeline](https://github.com/Ewuack/cloud-sdlc-pipeline) | CI/CD pipeline with security gates |

---

**Author:** Erick Guacamaya — Cloud Technical Program Manager
**LinkedIn:** [linkedin.com/in/erickguacamaya](https://linkedin.com/in/erickguacamaya) | **GitHub:** [github.com/Ewuack](https://github.com/Ewuack)
