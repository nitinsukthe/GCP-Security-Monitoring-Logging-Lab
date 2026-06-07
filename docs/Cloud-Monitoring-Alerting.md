# Cloud Monitoring Alerting

## Objective

To create a monitoring policy capable of detecting cloud resource activity using custom security metrics.

## Monitoring Service

Google Cloud Monitoring

## Alert Policy

Policy Name:

GCE VM Activity Alert

## Data Source

vm_activity_metric

## Configuration

Condition Type:

Threshold

Trigger:

Any Time Series Cross Threshold

Threshold:

Greater Than 0

## Alert Workflow

Audit Logs
→ Log-Based Metric
→ Cloud Monitoring
→ Alert Policy

## Validation

The alert policy successfully detected metric activity generated from Compute Engine operations.

## Security Benefits

- Real-time activity monitoring
- Early detection of infrastructure changes
- Security event visibility
- Incident response support

## Outcome

Successfully implemented cloud-native detection and alerting capabilities within GCP.
