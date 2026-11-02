# Daily check-in: "what needs me?"

The admin wants to know, in a minute, whether anything is broken, waiting on them, or about to run out.

## Calls

1. `account_overview`: the one-call summary. Its answer says which tool gives the detail behind each count.
2. `inbox_list` with the replies queue: prospects' replies nobody has answered yet. The overview does not include them, and they are often what matters most.
3. If the admin asks about failed or stuck work, `status_get` with no job named.
4. For a Monday or weekly check-in, add `report_campaign_performance` for last week with the comparison, so the brief says how the week went.

Answer with what the question needs; do not call every tool by reflex.

## Shape

Use the [daily brief template](../assets/templates/daily-brief.md): the count of things that need the admin first, then Fix, Reply and review, Since yesterday, and one next step. Each item keeps its console link. Do not mark notifications read unless the admin asks.
