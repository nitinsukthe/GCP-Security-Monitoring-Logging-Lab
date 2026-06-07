# Cloud Audit Logs Analysis

## Objective

To investigate administrative and operational activities occurring within the Google Cloud environment using Cloud Audit Logs.

## Service Used

Google Cloud Logging

## Log Source

Cloud Audit Logs

## Query Used

resource.type="audited_resource"

## Analysis Process

1. Opened Logs Explorer.
2. Configured audit log filters.
3. Expanded time range to include recent activity.
4. Reviewed recorded audit events.
5. Identified service operations and administrative actions.

## Observed Events

The following event types were observed:

- EnableService
- GetOperation
- Cloud OS Config Activity
- Service Usage Operations
- Billing Configuration Updates

## Security Value

Audit logs provide:

- Accountability
- Administrative activity tracking
- Incident investigation evidence
- Change monitoring
- Compliance reporting

## Findings

Cloud Audit Logs successfully captured project-level administrative actions and API activity.

## Recommendations

- Retain audit logs for security investigations.
- Monitor privileged administrative actions.
- Export logs to a SIEM for long-term retention.
- Create alerts for high-risk activities.
