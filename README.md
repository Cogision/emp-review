# EMP Review

EMP Review supports structured assessment of scientific publications using the Evidential-Maturity Profile (EMP).

## Current application: v0.25.0

[Open EMP Review](https://emp-review-focal.dw1975.chatgpt.site)

Version 0.25 adds comparison of two to five AI analyses of the same text, a source-grounded recommended draft with preserved originals, and visible deletion controls for completed reports. Claim identity and scope changes are flagged separately from differences in assessment.

## Source archives

| Version | Download | Source commit |
| --- | --- | --- |
| **v0.25.0** | [Source ZIP](archives/emp-review-v0.25.0-source.zip) · [Checksums and metadata](archives/emp-review-v0.25.0-source.json) | `286761ca039b710820aa824f9e6890f7c3284cc6` |
| v0.17.0 | [Source ZIP](archives/emp-review-v0.17.0-source.zip) | `a6b0df98c07221445af4928bfb74f7646c0bba7d` |

v0.25.0 ZIP SHA-256: `1b25836e8557f808d9e9dd9fb119f2f0bb3aa36a2fdaba65a594234414bde9ef`.

v0.17.0 ZIP SHA-256: `bd09de6d94fe28630660e43d8328404fb71d6b13c11cc3a7c1c53bd4c94d272f`.

The v0.25 archive includes application code, the dependency lockfile, tests and database migrations through 0011. Extract it and read `PUBLIC_SOURCE_NOTES.md` and the application `README.md`.

The deployed source includes a private, owner-specific pilot bundle of supplied full-text papers, original PDFs and assessments. In the public v0.25 archive, `lib/pilot-import-data.server.json` is replaced with `[]`. The optional preloaded pilot and its dataset-dependent tests require that separately retained private bundle. Existing data in the live application is unchanged.

Source archives exclude runtime secrets and do not back up user accounts, uploaded reports or the live database. The hosting manifest records the original Site identity and must be adapted before deploying an independent copy.

## Earlier applications

- v0.17: the comprehensive review workflow remains at https://emp-review-mvp.dw1975.chatgpt.site.
- v0.18 introduced the focal workflow at the current application's address. That application has since advanced to v0.25.0.
