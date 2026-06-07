# Cleanup Steps

## Objective

Remove deployed resources after project completion to avoid unnecessary cloud charges.

## Resources Removed

### Compute Engine VM

Resource:

monitoring-test-vm

Action:

Deleted

### Cloud Monitoring Alert Policy

Resource:

GCE VM Activity Alert

Action:

Deleted

### Log-Based Metric

Resource:

vm_activity_metric

Action:

Deleted

### Optional Project Shutdown

Project:

gcp-security-monitoring-lab

Action:

Project scheduled for shutdown after completion.

## Verification

Confirmed that:

- VM resources were removed.
- Alert policies were removed.
- Log-based metrics were removed.
- No active cloud resources remained.

## Outcome

Environment successfully cleaned up and secured against unintended costs.
