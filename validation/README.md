# Validation record

## Demonstrated in the Azure lab

| Check | Result | Evidence |
|---|---|---|
| `AzureActivity` coverage query | 43 records; 2026-10-11 01:31:14 UTC to 2026-10-12 06:09:28 UTC | Screenshot 02 |
| Successful tag-write hunt | Three successful writes returned | Screenshot 03 |
| Scheduled analytics rule | Enabled; Informational; hourly frequency and one-hour period; validation passed | Screenshots 04 and 05 |
| October 12 test timeline | Start at 04:30:50.350 UTC; Success at 04:30:51.631 UTC | Screenshot 06 |
| Alert and incident path | Two planned test events resulted in two alerts and two incidents | Screenshots 07 through 13 |
| Analyst disposition | Both incidents closed as Benign Positive - Suspicious but expected | Screenshots 10 and 11 |

## Not validated

- No real malicious activity, containment, recovery, or automated response was performed.
- No role-assignment detection was deployed or tested.
- No deletion detection was deployed or tested against a disposable resource.
- Incident entity mapping is absent; the two incidents show no mapped entities.
- Budget notification delivery is not shown; the budget screen shows no action group.
- Attribution of the earliest successful tag write remains unresolved in the report.

The KQL files are query examples for a workspace with compatible Azure Activity Log data. Validate operation names and schema in the target workspace before using proposed queries as analytic rules.
