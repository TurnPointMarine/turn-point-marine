# Turn Point Marine Engine

Vessel maintenance management tool for Turn Point Marine (TPM). Hosted at client.turnpointmarine.com via Azure Static Web Apps, deployed automatically from main branch commits.

## Stack
- Plain HTML / CSS / JS, no framework, no build step
- Per-vessel JSON data files
- QuickBooks Online for invoicing — materials parser handles QBO invoice text format

## Vessels
Undaunted, Hannah-Mae, Moondance (engine in development), Salish-See (engine in development), Whistler

## Project conventions
- Date format: YYYY-MM-DD
- M/S (materials/services) rows take dollar input, not hours
- Materials sort below labor by default
- Holding Pattern section is purple, sits above Authorization Needed, excluded from client export and totals
- GitHub commit history is the backup — no separate backup mechanism (backupjsons folder is supplemental)

## Deploy
- Commits to main → Azure Static Web Apps redeploys automatically
- Test locally by opening index.html in a browser before committing

## Active TODO
- PA signature → OneDrive integration
- URL tokens
- Moondance engine (use Undaunted as template)
- Salish-See engine
- Mobile signing
- Template v3

## How I work
- Plan before non-trivial changes — show me what you'll touch before doing it
- Don't refactor unrelated code while making a focused fix
- When unsure about a vessel-specific convention, ask rather than guess
