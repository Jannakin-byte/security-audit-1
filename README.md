# security-audit-1

## Cybersecurity Projects

- [Botium Toys Security Audit (NIST CSF)](https://github.com/YOUR_USERNAME/botium-toys-security-audit)  
  A fictional internal security audit based on NIST CSF, focused on risk analysis, compliance (GDPR, PCI DSS), and actionable controls.

## Audit Scope & Goals

**Scope:**  
This internal audit covers Botium Toys’ physical location and online infrastructure, including payment systems, customer databases, and EU data processing operations.

**Goals:**
- Identify and document existing security controls
- Assess compliance with PCI DSS (for payment processing) and GDPR (for EU customer data)
- Reduce business risk through mitigation of vulnerabilities
- Provide recommendations for improving the security posture

## Assets Reviewed

| Asset Type                | Description |
|--------------------------|-------------|
| Payment Gateway          | Online checkout system via third-party processor |
| Customer Database        | Stores user data (names, addresses, emails, order history) |
| Internal Network         | Local office network, employee devices, POS systems |
| Website & E-commerce     | Public-facing web application hosted on AWS |
| Employee Credentials     | Email, cloud service logins, and admin panel access |
| Data Backups             | Stored on local NAS and cloud |

## Risk Assessment Summary

| Risk Category           | Description | Likelihood | Impact | Risk Level |
|------------------------|-------------|------------|--------|------------|
| Weak Password Policies | Employees use weak or reused passwords | High | High | Critical |
| Lack of MFA            | No MFA enabled for admin or cloud access | Medium | High | High |
| GDPR Non-Compliance    | No user data deletion or access request policy | High | High | Critical |
| Unpatched Software     | POS and local machines not regularly updated | Medium | Medium | Medium |
| Insecure Backups       | No encryption or off-site redundancy | Low | High | Medium |

## Controls & Compliance Checklist

### Identity and Access Management
- [ ] Enforce strong password policies
- [ ] Enable multi-factor authentication (MFA)
- [x] Role-based access control (RBAC) implemented

### Data Protection
- [ ] Encrypt customer data at rest and in transit
- [ ] Implement GDPR rights (data access, deletion)
- [x] HTTPS enforced on all web pages

### Regulatory Compliance
- [ ] Maintain PCI DSS compliance checklist
- [ ] Assign a Data Protection Officer (DPO) for GDPR
- [ ] Create data retention and deletion policy

### System Maintenance
- [ ] Apply software patches regularly
- [x] Firewall and antivirus solutions in place
- [ ] Monitor logs for suspicious activity

## Recommendations

1. **Enforce MFA** across all critical systems and user accounts.
2. **Establish GDPR procedures**, including user data requests and deletion.
3. **Encrypt all backups** and store off-site copies securely.
4. **Update all devices** and POS systems with latest patches.
5. **Educate employees** through regular cybersecurity training sessions.

## Appendix

- **Framework Used:** NIST Cybersecurity Framework (Identify, Protect, Detect, Respond, Recover)
- **Compliance Focus:** PCI DSS, GDPR
- **Author:** Jacob Akins
- **Date:** May 2025

> *Note: This is a fictional scenario used for educational purposes as part of cybersecurity training.*
