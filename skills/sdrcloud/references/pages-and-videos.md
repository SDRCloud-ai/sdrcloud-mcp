# Making pages and videos with someone

Work the way a good designer works with a client: get the job in one pass, put a first version in front of them fast, then change what they point at and show it again. Each round should take one message from them and one answer from you.

## The loop

1. **Get the job.** What it is for, who receives it, and the one thing the reader should do (book a call, watch, reply). If the request says enough to guess sensibly, build now and list what you assumed. Ask first only for what you cannot guess and that would change the whole thing (see conversation.md).
2. **Start from what exists.** `search` for their pages and videos. If one already does a similar job, offer to start from a copy (read it, then create a new one from its blocks or scenes) instead of from nothing.
3. **First draft fast, in their look.** `brand_get` for colours, fonts and logos; never ask about colours, fonts or layout. Write real copy for their offer, not lorem ipsum, and keep their own wording where they gave it.
4. **Show every version** in the shape of [the draft update template](../assets/templates/draft-update.md): what changed in a line, the pictures, the preview link, what is still missing, and two or three numbered next changes.
5. **Change what they point at.** Make all the changes in one message in one update, keeping the rest. Free previews have a daily allowance, so do not spend one on each small tweak, and never save a change only to look at something.
6. **Finish when they say it is done.** Ask "Ready to use it in campaigns?" when it looks finished; on a yes, finish it, then say where to pick it in a campaign in the console.

## What SDRCloud pages look like

Real pages are long and follow one shape, so use it when the person does not describe one:

- a header with the logo first and a footer last;
- an opening section that greets the prospect by name, with one clear button;
- a personalised video near the top (three in four pages carry one, often the account's own video template);
- proof: benefits side by side, cards, a testimonial, a scrolling banner of logos or claims;
- a booking calendar or a second button to book;
- most often thirteen sections in all.

A button needs a real destination. If you do not have their booking link, say so with the draft and ask for it; never invent one.

## Personalisation

- Use the account's own field names. Read the variables of one of their existing pages or videos and reuse them; `{{firstName}}` and `{{company}}` are the most common. The same field is spelt differently in different accounts ({{firstName}} in one, {{first_name}} in another), so never guess a spelling when an existing template shows it.
- Name any new field you add ("this uses `{{painPoint}}`; your leads need that column") so the person knows their lead list must have it.
- Previews use made-up sample values. Say whose ("shown for a sample: Dana at Acme") and never fill a preview with a real prospect's details unless the person asks for that person.

## Pictures

- Pictures come from their image library (`media_list`) or from a public https link (`media_import`, one call per picture).
- A photo on their computer, or one they attach to this chat, cannot be brought in. Say so in one line and offer the two ways that work: add it to the image library in the console and tell you its name, or send a public link. Meanwhile keep a library picture or the current one in its place, and say which.
- Prefer their logo and brand pictures from `brand_get` over stock images.

## Videos

- **What makes them personal.** Many SDRCloud videos show each prospect their own website: a website scene whose address is a field such as `{{website}}`, scrolled while the narration talks. Three to five scenes is usual: their site, a picture or clip of the offer, and a close.
- **A real site for the samples.** Previews and test renders of a website scene need a real public site, or they show an empty page; never use example.com or a made-up domain. Use the site they gave; otherwise pick the public site of a well-known company like their prospects, name it as the sample ("shown on <that site> as a sample"), and offer to swap in their own. Never hold the work back to ask for one.
- **Narration sets the length.** A narrated scene lasts as long as its speech. Before calling a length final, play the script with `video_narration_preview` and give the length it returns, as "about": the same text can come out a second or two longer or shorter in the real render.
- **Voices.** From `video_voices_list`, offer two or three that fit what they asked ("warm, female"), with sample links where there are, and say the voice changes the test render's price. For their own voice, they record it in the console or give a link to an audio file.
- **What the stills cannot show.** A scene still shows only where a website scene starts, and no motion or sound; a clip scene may have no still. Say so in a line with each video draft, and do not change a scroll or a length just to see another frame.
- **The real thing.** A test render is for when the script, voice and scenes are settled, not for each tweak. It costs credits and takes a few minutes: tell them, follow with `status_get`, then show the video link, its landing page and the poster.

## Real pages and test renders

When they ask for a real page or a test render, make the price call in that same turn, and answer in one message with the price, the balance, and the exact values it will use (name, company, website), plus anything still missing. Fill anything they have not given with a named real default (a sample person, and a real site as above) so that a plain yes can go ahead, and say they can change it. Never ask for a yes without the price, and never spend on values you did not show them.

The real page's link is the one to send. Opening it yourself won't count as the prospect's visit, so give the link without warning about it.

## When a change is refused

- A template a live campaign uses cannot be changed from here, because the change would reach that campaign's prospects. The answer names the campaign: offer a copy as a new template.
- A daily allowance reached, a price that moved or a balance too low spends nothing. Say what the answer says and when it can be tried again, and offer to carry on with what is free.
