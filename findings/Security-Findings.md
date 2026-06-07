# Security Findings

## Project

GCP Security Monitoring and Logging Lab

---

# Finding F-01

## Title

Project Owner Assigned Full Administrative Permissions

### Severity

Medium

### Observation

The project user account was assigned the Owner role.

### Risk

The Owner role provides unrestricted access to all project resources, IAM permissions, billing configurations, and security settings.

### Impact

Compromise of an Owner account could result in:

* Resource deletion
* Privilege escalation
* Security control modification
* Data exposure

### Recommendation

Implement the Principle of Least Privilege (PoLP).

Assign only the permissions required for job responsibilities.

---

# Finding F-02

## Title

Default Compute Engine Service Account Uses Editor Role

### Severity

High

### Observation

The Compute Engine default service account was assigned the Editor role.

### Risk

The Editor role grants broad permissions across multiple Google Cloud services.

### Impact

If a VM is compromised, an attacker may inherit excessive permissions through the service account.

### Recommendation

* Create dedicated workload identities.
* Replace Editor permissions with custom least-privilege roles.
* Restrict service account permissions to operational requirements.

---

# Finding F-03

## Title

Security Command Center Not Available

### Severity

Informational

### Observation

Security Command Center requires an organizational environment and was unavailable in the personal project.

### Impact

Advanced posture management features could not be tested.

### Mitigation

Alternative monitoring controls were implemented:

* Cloud Logging
* Cloud Audit Logs
* Log-Based Metrics
* Cloud Monitoring Alert Policies

---

# Conclusion

The project successfully identified IAM-related security risks and demonstrated alternative monitoring controls using native Google Cloud security services.
