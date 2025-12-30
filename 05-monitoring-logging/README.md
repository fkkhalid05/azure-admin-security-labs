# Monitoring & Logging Lab

## Objective
Implement monitoring, logging, and alerting to gain visibility into Azure resources, detect issues, and support security investigations.

## Architecture
- Azure Monitor
- Log Analytics Workspace
- Activity Logs
- Resource Logs
- Alerts and Action Groups

## Design Decisions
- Centralized logs in a Log Analytics workspace
- Enabled platform and resource logging for visibility
- Used alerts to proactively detect issues
- Retained logs for troubleshooting and security auditing

## Steps
1. Created a Log Analytics workspace to centralize logs and metrics.
2. Enabled Azure Activity Logs to track subscription-level changes.
3. Configured resource diagnostic settings to send logs and metrics to Log Analytics.
4. Queried logs using KQL to analyze activity and identify issues.
5. Created alerts based on metrics and log queries.
6. Tested alerting and validated log ingestion.

## Security Considerations
- Activity logs help detect unauthorized changes
- Centralized logging supports incident response
- Alerts reduce mean time to detect (MTTD)
- Log retention supports auditing and compliance requirements

## On-Premises Mapping
- Event Viewer → Azure Monitor Logs
- SIEM (Splunk / QRadar) → Azure Monitor / Sentinel
- Syslog → Log Analytics
- SNMP / monitoring tools → Azure Monitor metrics

## Lessons Learned
- Monitoring without alerts is reactive, not proactive
- Centralized logging simplifies troubleshooting
- Logs are critical for security investigations
- Misconfigured resources are easier to detect with visibility enabled
