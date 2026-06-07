# Risk Assessment

## Project

GCP Security Monitoring and Logging Lab

---

# Risk Matrix

| Finding                                  | Likelihood | Impact | Risk Level    |
| ---------------------------------------- | ---------- | ------ | ------------- |
| Owner Role Assignment                    | Medium     | High   | Medium        |
| Default Service Account Uses Editor Role | High       | High   | High          |
| Security Command Center Unavailable      | Low        | Low    | Informational |

---

# Risk Analysis

## Owner Role Assignment

### Threat Scenario

An attacker compromises an account with Owner permissions.

### Potential Impact

* Resource destruction
* Billing abuse
* Privilege escalation
* Security policy modification

### Recommended Control

Apply least privilege access.

---

## Default Service Account Uses Editor Role

### Threat Scenario

An attacker gains access to a Compute Engine instance.

### Potential Impact

* Unauthorized API access
* Lateral movement
* Resource manipulation

### Recommended Control

Implement dedicated service accounts with minimum required permissions.

---

# Overall Risk Rating

Medium

The environment demonstrated acceptable security monitoring controls; however, IAM permissions should be hardened before production deployment.

---

# Security Maturity Assessment

| Domain                | Status                |
| --------------------- | --------------------- |
| Logging               | Implemented           |
| Monitoring            | Implemented           |
| Alerting              | Implemented           |
| Detection Engineering | Implemented           |
| IAM Hardening         | Needs Improvement     |
| Security Governance   | Partially Implemented |

---

# Final Assessment

The project successfully implemented cloud-native monitoring, audit logging, and alerting controls. Future improvements should focus on IAM hardening, workload identity management, and organization-level security services.
