# IAM Security Review

## Objective

To review user and service account permissions and identify security risks.

## IAM Components Reviewed

### User Account

Role:

Owner

Purpose:

Administrative access to project resources.

### Compute Engine Default Service Account

Role:

Editor

Purpose:

Default service account used by Compute Engine resources.

## Security Findings

### Finding 1

Owner Role Assigned

Risk:

The Owner role provides unrestricted administrative privileges.

Recommendation:

Apply the Principle of Least Privilege and assign only required permissions.

### Finding 2

Default Service Account Assigned Editor Role

Risk:

Editor permissions are broad and may increase impact if compromised.

Recommendation:

Replace Editor with custom least-privilege roles.

Use dedicated service accounts for workloads.

## Security Impact

Overly permissive IAM roles increase the attack surface and can enable privilege escalation.

## Outcome

Successfully identified IAM security improvement opportunities within the project.
