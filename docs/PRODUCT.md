# Product brief and next steps

## User and job to be done

An individual freelancer working across several platforms wants to see how much they worked, what was approved and what has actually been settled, without manually reconciling scattered platform dashboards.

## First usable workflow

Create a project → log work → mark work approved → record a payout → review the outstanding balance.

## Deliberate scope decisions

- Manual entry first: validate the workflow before API integrations.
- No tax calculation or income guarantee.
- Keep currencies separate; do not imply an exchange rate.
- Keep historical session rates stable.
- Preserve rejected work to reveal unpaid effort.
- Personal data stays in the browser; demo data is fictional and separate.
- No accounts, backend, bank connections or platform scraping in v0.1.

## Known limitations

- Payouts are project-level settlements; they do not link to specific sessions.
- No fee or currency-conversion reconciliation.
- No cross-device sync or simultaneous-tab conflict resolution.
- Dashboard earnings cover all time; the activity chart covers seven days.
- No running timer, CSV import/export or project archiving yet.
- Automated checks cover the model, not a full browser regression suite.
- Local storage is not an encrypted vault; backups are plain JSON.

## Proposed development backlog (not implemented)

1. **Date ranges and reporting.** Compare a week/month, clarify work dates versus payout dates, and export monthly totals.
2. **Effective hourly earnings.** Show approved earnings divided by all time invested, including rejected work. Explore tracking unpaid onboarding and revision time.
3. **Payout allocations.** Link a payout to selected sessions; support partial settlement without losing auditability.
4. **Fees and FX.** Preserve gross project earnings while recording fees, net receipt and user-entered exchange rates.
5. **Work entry improvements.** Timer, duplicate entry and CSV export; prevent accidental timer overlap.
6. **Project archiving.** Hide inactive projects while preserving all financial records.
7. **Accessibility and reliability.** Keyboard testing, storage failure recovery and conflict handling across browser tabs.

## Questions for the first real-use review

- Do approval states match the freelancer's actual platform workflow?
- Are hours sufficient, or do some projects require task-based fees?
- Does the user receive project-specific payouts or one combined platform payout?
- Is a paid/unpaid distinction sufficient, or are submitted invoices and expected dates needed?
- Which daily action is useful enough to make this preferable to a spreadsheet?

## AI-assisted development and evaluation

This prototype was implemented with ChatGPT assistance. Future Claude Code development can address the backlog above; do not describe this existing implementation as having been built with Claude Code. Keep a genuine development history and document observed behavior and changes. Any programme-specific response ratings must be written by the participant in accordance with that programme's rules.
