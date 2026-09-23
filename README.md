# Ontario SMB Problem Atlas

A cited, living map of what small businesses in Ontario struggle with, and the small tools being built to fix the ones software can fix.

Most "AI for small business" projects start with a technology. This one starts with a problem, a number, and a source.

*Last updated: 2026-09-23. Maintained by [Praju](https://github.com/prajuvin) of YHWH Digital, Toronto.*

## What small business owners report

| Problem | Figure | Source |
| --- | --- | --- |
| Total tax burden | 74% name it a top concern | [CFIB survey](https://www.cfib-fcei.ca/en/research-economic-analysis/our-members-opinions), Q4 2025, 8,511 responses |
| Labour shortages | 54% | CFIB survey |
| Government regulation and paperwork | 54% | CFIB survey |
| Trade challenges | 43% | CFIB survey |
| Crime and safety | 35% | CFIB survey |
| Inflation | 41.6% of businesses, the top obstacle | Statistics Canada survey, Q3 2026, via [a summary](https://www.bridginglocal.com/post/canadian-business-conditions-q3-2026) |
| Recruiting skilled employees | 25.2% | same |
| Cost of inputs | 24.1% | same |
| Cost of insurance | 22.4% | same |
| Owners who would not recommend starting a business now | more than 55% in Ontario and Canada | [CFIB, April 2026](https://www.cfib-fcei.ca/en/media/more-businesses-have-been-closing-than-opening-in-ontario-and-canada-were-in-an-entrepreneurial-drought) |

CFIB also reports six straight quarters of more business closures than openings. In Ontario it cites an exit rate of 6.7% against an entry rate of 5.1%.

One in four Canadian businesses plans to adopt AI within a year. The most common planned uses are data analytics (41.7%), large language models (39.3%), and chatbots (31.8%).

The full dataset, with as-of dates and confidence notes, is in [`data/problems.csv`](data/problems.csv).

## What gets built from it

Not every problem is a software problem. Tax burden is a policy issue. Paperwork, staffing knowledge, and missed inquiries are things a small tool can help with. Each build below answers one problem and ships with a tested result.

| Build | Problem it answers | Status |
| --- | --- | --- |
| `tender-radar` | Small vendors miss public tenders buried in large government feeds | Planned |
| `front-desk-agent` | Service businesses lose bookings when nobody answers messages | Planned |
| `compliance-calendar` | Owners lose time tracking regulatory obligations and deadlines | Planned |
| `sop-to-onboarding` | New hires take too long to train when procedures live in the owner's head | Planned |

Each build repo follows the same README structure: the problem in one plain sentence, who has it and the cited number, a demo, how it works, who tested it and what happened, how to run it, and what comes next.

## Related signals

Y Combinator's Fall 2026 Requests for Startups includes AI-Native Compliance Infrastructure and A Cloud for Small Software, both close to the problems above. See [`METHODOLOGY.md`](METHODOLOGY.md) for how sources are chosen and rated.

## Known gaps

- Owner-level voice is thin. The current evidence is survey-level. Interview notes and public forum threads are being added.
- The Statistics Canada figures come from a secondary summary; they will be replaced with the official release.
- Open challenges from Innovative Solutions Canada have not been reviewed yet.

## Contribute

Spotted a problem with a real source behind it? Open an issue with the claim, the number, and the link. Corrections to any figure are welcome.
