# Cold Call Brief — Cold Call Script & Prospect Brief Agent

Built by Epic Innovations, Inc. for B2B technology sales reps who want researched, specific cold call preparation instead of generic scripts.

## What this is

A Claude skill that builds a cold call brief for a single prospect. You give it the prospect's company name and LinkedIn profile, and it researches both and returns a formatted Word document with four sections:

1. **Conversation openers.** Permission-based openers built on verified recent events, such as company announcements, competitor moves, job postings, funding, and industry news.
2. **Suggested questions.** Diagnostic discovery questions in the order to ask them, with listening cues and follow-ups.
3. **Objection handling.** The likely objections, the calm response to each, and the next step.
4. **Closing checklist.** What to confirm and do before the call ends, including booking the meeting while the prospect is still on the line.

The goal of every call is to book a 20 to 30 minute discovery meeting. The brief is built around that goal, not around pitching the product.

## What makes it different

- **It learns from your calls.** A swipe file collects industry, persona, and company research with sources and dates, so each brief is faster to prepare and more specific than the last. A feedback log records which openers and objection responses work, and future briefs reflect those results.
- **It works from your offer.** On first use it asks what you sell, who you sell to, and your proof points, then uses that in every brief.
- **It is built on a documented method.** The framework draws on the B2B tech cold calling method in the source material. Your own results can override it.

## Setup (5 minutes)

1. Copy this whole `cold-call-brief` folder into the location your Claude surface loads skills from.
2. Start a conversation and ask Claude to prepare a cold call brief. On the first run, it will ask for your seller profile (what you sell, to whom, and proof points) and save it to `data/seller-profile.md`.
3. Have the prospect's company name and LinkedIn URL ready. If LinkedIn blocks access, which it often does, Claude will ask you to paste the key details from the profile.
4. Receive the brief as a Word document. Review it before the call.
5. After your calls, tell Claude what happened. It will record the results in `data/feedback-log.md` and use them in future briefs.

## Folder contents

| Path | Purpose |
|---|---|
| `SKILL.md` | The skill's instructions and workflow |
| `references/framework.md` | The cold call method, openers, objection responses, and common mistakes |
| `references/linkedin-signals.md` | Which profile and job-posting signals make good triggers, and how to verify them |
| `templates/brief-template.md` | The layout of the finished brief |
| `data/seller-profile.md` | Your offer, target buyers, and proof points |
| `data/swipe-file.md` | Accumulated research by industry, persona, and company |
| `data/feedback-log.md` | Call outcomes by opener and objection |

## Privacy

Prospect research, your seller profile, the swipe file, and the feedback log are yours. They stay in your own Claude conversations and in this folder. The skill does not send that material to any service other than your Claude session, and it is not intended to train or build third-party models. Research done with web search sends search queries to the search provider, so do not put confidential details in queries.

## Before you use the brief on a call

Every brief is a starting point. Before you use it:

- Check every trigger against its source. Do not open with a fact you cannot confirm.
- Make sure the openers sound like you. A brief you can't say naturally will not work on a call.
- Follow the calling, recording, and data rules that apply where you and your prospect are located. This skill does not provide legal or compliance advice.

## License and terms

© 2026 Epic Innovations, Inc. All rights reserved. This repository is shared free of charge under specific terms. See [LICENSE.txt](LICENSE.txt) and [TERMS_OF_USE.md](TERMS_OF_USE.md) before using or sharing it. In short: free to download and use for your own sales work, not free to resell, rebrand, or redistribute as your own.
