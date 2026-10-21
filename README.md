# dependency-audit-pilot

Pilot repository for automating the dependency audit checklist.

## Why this exists

Today the dependency and security audit checklist is run by hand: someone has to
remember to check pinned dependency versions, look for newly published security
advisories, and write up findings before anything can be acted on. This repo is
the landing spot for moving that work to automation so the audits keep running
automatically instead of by hand.

## What it should do

- Automatically and regularly scan dependencies for known vulnerabilities and
  outdated versions.
- Surface findings as actionable issues or pull requests instead of a
  hand-written checklist.
- Keep a standing, dated record of audit results so the recurring "state of my
  open-source corner" brief can be assembled from data rather than memory.
- Act as a repeatable place to pilot delegating remediation work to GitHub's
  Copilot coding agent.

## Where to start

See the tracking issue **"Automate the dependency audit checklist"** in this
repository's issue tracker.

## Notes

- This repository was created as a fallback: no repository under the HeziLiu
  personal account could accept the issue (issue creation was rejected with
  `403 Resource not accessible by personal access token` on the two
  issue-enabled source repositories, and the two remaining repositories are
  forks with the issue tracker disabled).
- Dependabot alert data was not retrievable for the personal-account source
  repositories (same 403), and Dependabot alerts are disabled on both forks.
  Enabling and wiring up alert access is a natural first task for the audit
  automation itself.
