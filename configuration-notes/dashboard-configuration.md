
---

# configuration-notes/dashboard-configuration.md

```markdown
# Dashboard Configuration

## Objective
Create a custom SOC dashboard in Wazuh/OpenSearch Dashboards.

## Dashboard Name

```text
Harshil's Dashboard
# configuration-notes/dashboard-configuration.md

```markdown
# Dashboard Configuration

## Objective
Create a custom SOC dashboard in Wazuh/OpenSearch Dashboards.

## Dashboard Name

```text
Harshil's Dashboard

## Visualizations Created

1. Total Alerts per Day
  Visualization type: Bar chart
  Index: wazuh-alerts-*
  Metric: Count
  X-axis: Date histogram
  Field: timestamp
  Interval: Daily
2. Top 5 Security Rules Triggered
  Visualization type: Donut chart
  Index: wazuh-alerts-*
  Metric: Count
  Split slices: Terms
  Field: rule.description
  Size: 5
3. Agent Status Overview
  Visualization type: Data table
  Index: wazuh-monitoring-*
  Fields used:
  agent.name
  status
  count
