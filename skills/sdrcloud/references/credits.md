# Credits

SDRCloud credits pay for the agents' work. When they run out, campaigns stop sending.

## Calls

- "How many credits do I have?", "When will I run out?": `credits_get`.
- "What spent my credits?", "Why did spend jump?", "I'm worried about credits": `credits_get` with balance and spend together, for the period the admin means (the last 30 days by default).
- "Show me the charges" or grants: `credits_get` with activity.

## Shape

- Lead with the runway: "About {n} days of credits left at the current pace" (or that it cannot be projected yet, with the tool's reason).
- Then the balance as the tool splits it: what can fund new work, and what is held for work in progress. Do not add them up.
- Say whether it is in the warning or critical range, as the tool classifies it.
- Spend as a small table, biggest first: kind of work or agent, credits, share of the total.
- Buying credits happens in the console: give the link, never offer to buy.

## Pages and test videos

- Making and changing page and video templates, and their previews, cost no credits. Previews have a daily allowance; the tool says when one is used up.
- One real page for one person (`hvo_page_create`) and a test render (`video_test_render`) cost credits. The first call returns the price and the balance and spends nothing; give both, and repeat the call with `confirmCredits` only after the person agrees to that price.
- If the balance is too low, say so with the price and the balance, and give the console link to buy; carry on with the free work.
