# Reporting: results, comparisons, trends, client updates

## Picking the period

- Turn the admin's words into the tool's period: "last week", "this month", "the last 30 days", or explicit dates. Calendar periods for "week" or "month", rolling ones for "last N days". With no period, use the last 30 days for rates and comparisons and say so.
- Ask `report_campaign_performance` for the comparison in the same call; when the comparison is not the period before (October against September), pass both sets of dates. `report_conversions` has no comparison: call it twice with explicit dates.
- Say which dates you used, and say when the current period is not over yet.

## Calls

- Results and rates: `report_campaign_performance`, grouped by campaign, agent, day or week to match the question. Trends: group by day or week.
- Who converted and how: `report_conversions`.
- A client update, or "how did we do": both, with the same period and campaign.
- "Why did sends drop?": the results, then `campaign_check_readiness` for the campaign that dropped.

## Shapes

| Question | Template |
| -- | -- |
| Compare campaigns or agents | [campaign comparison](../assets/templates/campaign-comparison.md) |
| What changed, since last week, trending | [what changed](../assets/templates/what-changed.md) |
| Update for my client | [client update](../assets/templates/client-update.md) |
| A trend over weeks or days | a text bar chart ([visuals.md](visuals.md)) |

- Lead with the headline: the total and its direction ("Reply rate 8.2% over the last 30 days, ▲ 1.2 pts").
- A figure the tool returns as not available stays not available, with the tool's reason. Never compute a replacement.
