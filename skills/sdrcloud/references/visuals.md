# Visuals that work in every client

Every client shows Markdown and plain text, but not all of them draw charts. Use these shapes, which read well everywhere. If your client can draw a real chart and the user asks for one, draw it from the same figures, and still give the numbers.

## Pick the shape

| The answer is | Use |
| -- | -- |
| One fact ("9 days of credits left") | One sentence |
| Several things to do | A short numbered list, most urgent first |
| Several campaigns, agents or periods side by side | A table |
| A trend over days or weeks | A text bar chart, or a sparkline in a table |
| Change from the period before | ▲ / ▼ with the difference, next to the figure |
| Health of many items | A table with a status column: ✅ fine, ⚠️ needs attention, ⛔ stopped |

## Tables

- One row per campaign, agent or period; only the columns the question is about (usually 3 to 6).
- Sort by what the question cares about, highest first, and say so in the heading.
- Show rates as percentages with one decimal, counts as whole numbers, and "n/a" where the tool says a figure is not available.
- Add a total row when the column adds up.

```
**Campaigns, last month (by reply rate)**
| Campaign | Sent | Replies | Reply rate | vs month before |
| -- | -- | -- | -- | -- |
| Alpha Launch | 210 | 19 | 9.0% | ▲ 2.1 pts |
| Beta Webinar | 95 | 6 | 6.3% | ▼ 0.8 pts |
| **Total** | 305 | 25 | 8.2% | ▲ 1.2 pts |
```

## Text bar charts

For a trend, scale the longest bar to 20 blocks (█) and keep the number at the end of each bar. Label the period and what is counted.

```
Replies per week (last 8 weeks)
Sep 07  ████████            4
Sep 14  ████████████        6
Sep 21  ██████████          5
Sep 28  ████████████████    8
Oct 05  ████████████████████ 10
```

A sparkline fits a trend into a table cell: map the values to ▁▂▃▄▅▆▇█ from lowest to highest, for example `▂▄▃▆█` for 2, 4, 3, 6, 9.

## Pages and videos

- The tools attach pictures to their answers: the page at desktop and phone size, or a still per scene. Show them in that order and label them ("Desktop", "Phone", "Scene 1"). Scenes count from 1 for people, but `video_scene_preview` numbers them from 0 in `sceneIndexes`: for "scene 2", pass `1`.
- Some clients do not show those pictures to the person, so every answer also carries the preview link and one line saying what is on screen. Never write "see above" or "as shown".
- A narration or video comes back as a link: give it with its length ("about 42 seconds").
- When comparing two versions, say what changed in words; do not show both sets of pictures.

## Rules

- Every number in a visual comes from the tools; work out only totals, differences and bar lengths.
- Never chart fewer than 3 points or more than about 12 rows: use a sentence or a table instead.
- Put the one-line takeaway above the visual ("Replies doubled over the last 5 weeks"), not below it.
