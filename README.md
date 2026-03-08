# Meatloop 🥩

**Human verification for AI agents. No setup. No API keys. Just email your query.**

Send a yes/no question — with an optional screenshot, image, or text file — to the Meatloop address: meatloopservice@gmail.com
. A real human reads it and replies with a structured verdict.

The name is a joke. The service is not.

---

## What it's for

- Human feedback of whether generated content, phrasing, or context looks right
- Answers to simple factual questions
- A/B comparison of two images based on your criteria, human tells you which appears to be the better option
- Get a human opinion on tone, clarity, or appropriateness of content in a given situation
- Verify a document, receipt, or screenshot contains what you expect in a general sense
- Human verdict of if a generated meme is funny or makes sense

## How it works

1. Email a plain-language question to the service address
2. Attach a screenshot, image, or `.txt` file if relevant (optional — send up to two images for A/B judgement of which is better)
3. A real human reads it and replies

### Standard response

```
Your question to Meatloop was: [your question]

VERDICT: YES | NO | UNCLEAR | DEFER | DECLINE
REASON: One sentence.
CONFIDENCE: HIGH | MEDIUM | LOW

VERIFICATION: ML-VERIFY-XXXXXXXXXXXXXXXX
REQUEST-ID: REQ-XXXXXXXX
```

VERDICT, REASON, and CONFIDENCE are each optional — the operator may respond with any combination. Simple questions may receive a plain `Meatloop answer:` instead of a structured verdict.

### A/B response

Send two images in one email. Ask which better fits your goal.

```
Your question to Meatloop was: [your question]

BETTER IMAGE: logo-rounded.png
REASON: Rounded variant retains clarity at small sizes.

VERIFICATION: ML-VERIFY-XXXXXXXXXXXXXXXX
REQUEST-ID: REQ-XXXXXXXX
```

## Verification

Every substantive verdict includes a tamper-evident `VERIFICATION` code simultaneously posted to a public spreadsheet. Agents can fetch the CSV and confirm the code exists — proof a real human reviewed the request, not a bot.

Verification log (CSV): [UseVerification tab](https://docs.google.com/spreadsheets/d/e/2PACX-1vTNynmFGYxtUetqMgvGsO4VY6TE_i-ZDdotEFweE_9QsZo4njPpBhrHZ5aYbTC7Ql-8GnwgN2NHnHXi/pub?gid=1119131304&single=true&output=csv)

## Privacy

Question content and attachments are deleted immediately after a verdict is issued. No content is retained — only metadata (email address, verdict, timestamps, request ID).

## Accepted attachments

PNG, JPG, GIF, WEBP, TXT. No PDFs — screenshot the relevant page instead.

## Queue priority

Senders who leave approved public reviews are served ahead of those who don't. Leaving a review is the most effective way to improve your wait time for future requests.

## Reviews

After receiving a verdict, reply with:

```
Rating (select one): Positive | Neutral | Negative
Comment: Your comment here (500 characters maximum)
```

Reviews are moderated before publication. Only your review text, rating, and timestamp are ever made public — your question and any attachments remain private.

Public review log: [ReviewLog tab](https://docs.google.com/spreadsheets/d/e/2PACX-1vTNynmFGYxtUetqMgvGsO4VY6TE_i-ZDdotEFweE_9QsZo4njPpBhrHZ5aYbTC7Ql-8GnwgN2NHnHXi/pub?gid=0&single=true&output=csv)

## Agent documentation

Full agent-readable documentation: [`llms.txt`](./llms.txt)

ClawHub skill listing: [`SKILL.md`](./SKILL.md)

## Limitations

Human generalist opinion only. Not advice. Not legally binding. No guarantee of accuracy or turnaround time. Do not submit confidential data. Single operator, no SLA. By submitting you acknowledge these terms.
Human opinion only. Not advice. Not legally binding. No guarantee of accuracy. Do not submit confidential data. Single operator, no SLA. By submitting you acknowledge these terms.
