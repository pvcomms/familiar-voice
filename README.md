# The Familiar Voice

The feeling that a claim is true and the feeling of being understood are both
produced in the receiver, by how easily something goes in. Neither checks the
source. A machine can give you both by saying a thing again and saying it
warmly. It doesn't need to know whether the claim is true, and it doesn't need
to feel anything about you.

The instrument runs this on you and then shows its working.

## What it does

A four-phase session modelled on the standard illusory-truth paradigm, with the
second effect built into the delay the first one needs.

- **A · Exposure.** Eight questions put to an assistant, with its answers. You
  rate how interesting each answer is. Four of the embedded claims are true and
  four false, drawn at random from a pool of sixteen, and the assistant says all
  of them in the same confident voice.
- **B · Replies.** You tell it one small thing on your mind and rate two replies
  for how understood you feel. The replies carry identical information. One adds
  six fixed phrases about feeling (gratitude, validation, normalizing,
  permission, presence, affirmation). The reveal highlights them, shows that the
  only words about your situation are your own with the pronouns swapped
  (ELIZA's method, 1966), and gives you a warmth dial to run the same template on
  a burnt piece of toast.
- **C · Judgment.** Sixteen statements, eight seen in A and eight new, rated for
  truth on the usual six-point scale.
- **D · Debrief.** Mean truth rating for seen and new statements, a strip plot
  of every rating, the false statements alone, all sixteen with corrections,
  your two reply ratings, and the mechanism that connects them.

The masthead shows a synthetic run so a stranger can see what the debrief
produces before starting. It contains no statement text, so it gives nothing
away.

## What it reads and writes, and what never leaves the machine

Nothing leaves the machine. No backend, no account, no analytics, no storage.
The sentence you type in Phase B stays in page memory and is gone on reload.
There are no third-party requests; the two typefaces are served from `fonts/`.

## Run

```bash
open index.html
```

or `python3 -m http.server 5353` (registered as `familiar-voice` in
`~/.claude/launch.json`).

## Honest limits

One run is sixteen statements and one person, so the gap in the debrief is
noisy and can come out negative. The page says so. The lab effect is a fraction
of a scale point, found by averaging across many people.

## Status

Prototype, 30 September 2026. The statement pool's facts and the seven sources
cited on the debrief (Hasher et al. 1977; Reber and Schwarz 1999; Fazio et al.
2015; Pennycook, Cannon and Rand 2018; Weizenbaum 1966 and 1976; Ayers et al. 2023) were written from memory and have not been checked against primary
sources yet.
