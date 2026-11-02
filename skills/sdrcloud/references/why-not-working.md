# Something is not working

Work out first what the admin is asking about, because each has its own tool:

| The admin says | It is about | Call |
| -- | -- | -- |
| "Why isn't Jane Doe getting emails?", "What's next for this lead?" | one lead | `lead_explain` with the lead's name or email |
| "Why hasn't the spring campaign sent anything?", "Why did my campaign stop?" | a whole campaign | `campaign_check_readiness` with the campaign name |
| "Why has nothing gone out today?" with no campaign named | the account | `account_overview`, then `campaign_check_readiness` for each campaign it shows paused or blocked |
| "Did the video for Sam finish?", "Is my HubSpot sync stuck?", "Anything fail this week?" | a long job | `status_get` with the kind and a name, or nothing to list recent failures |

## Leads

- A lead can be in several campaigns, and several leads can share a name. If the tool returns candidates, call it once per candidate and cover each, or ask which one; never pick one silently.
- If the lead is fine but its campaign is not sending, follow with `campaign_check_readiness` for that campaign and say so.
- An agent waiting on purpose is normal: say when the next email is planned.

## Campaigns

- Give every reason the tool returns, starting with the ones the admin can fix, and what fixing each one takes, with its console link.
- If the campaign is sending normally, say so plainly, with when it sends next.
- A short campaign name may match more than one campaign: cover each or ask.

## Jobs

- Say the state in plain words (finished, still running, stuck, failed) and, for a failure, the reason the tool gives.
- If the admin wants a job retried, point them to its console link.
- To check again later, pass back the job's handle.
