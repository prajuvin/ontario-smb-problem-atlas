# Roadmap

*Updated 2026-09-23.* Two builds work on real inputs and have tests. What neither has yet is a real user, so the next step is validation, not more features.

## Status

| Build | Problem | Status | Proof so far |
| --- | --- | --- | --- |
| [tender-radar](https://github.com/prajuvin/tender-radar) | Small vendors miss public tenders | **Working on real data** | 839 real open tenders; 18 unit tests; browser matches equal the Python matcher; no WCAG A/AA issues found |
| [front-desk-agent](https://github.com/prajuvin/front-desk-agent) | Service businesses lose bookings when nobody answers | **Working, AI not yet live** | 10 unit tests; browser test in 3 modes; unsafe AI output blocked; hand-offs reach the owner's webhook |
| compliance-calendar | Paperwork and regulation (54% of owners, CFIB) | Not started | |
| sop-to-onboarding | Labour shortages (54%, CFIB) | Not started | |

## Now (next 2 weeks)

- **Tender Radar:** turn on GitHub Pages, confirm the daily update runs, and show it to 3 Ontario vendors. Record which tenders they would have missed.
- **Front Desk:** add a rate limit, deploy to Praju's own Vercel account with an Anthropic API key, and test with real AI answers.

## Next (1 to 2 months)

- **Front Desk:** two-week trial with one local business. Measure questions answered, bookings passed on, and wrong answers.
- **Tender Radar:** free daily email for saved words, only if vendors ask for it.

## Later

- Owner login and message history for Front Desk (Supabase)
- Related-word matching and AI summaries for Tender Radar
- Start compliance-calendar, the most requested problem in the survey data

## Risks

| Risk | Plan |
| --- | --- |
| The government data server blocks GitHub's robot | The downloader already sends a browser-style identifier. If the robot is still blocked, run the update from another scheduler. |
| Front Desk costs grow if the demo is abused | Rate limit before any public link; demo mode stays off on client sites |
| Neither build finds a real user | That is the answer to learn; the atlas records it and the next problem gets picked |
