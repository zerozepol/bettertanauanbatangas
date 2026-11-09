# Better Tanauan

Independent community transparency portal for **Tanauan City, Batangas**, maintained by [@zerozepol](https://github.com/zerozepol). Work in Progress. Not an official LGU website and not yet registered with or endorsed by BetterGov.

## Run locally

No package installation is required. Build using `node build.mjs`, then run `python3 -m http.server 4173 --directory dist` and open http://localhost:4173. Node.js 18+ and Python 3 are sufficient.

## Scope

This is an independent repository, with its own initial commit, source, LGU data and build. No dependency on the previous shared portal or another LGU repository. Relative asset paths support both domain-root and subpath hosting.

Six sections follow the [BetterGov LGU guide](https://lgu.bettergov.ph/GUIDE): offices/services, barangays, officials, budget/expenditure sources, project records and ordinance archive. Adapted from the BetterSolano static HTML template. Upstream styles and component structures are retained, with LGU-specific content and the sourced directory behavior. See TEMPLATE.md and LICENSES/BetterSolano.txt for provenance and license details.

## Data

64 sourced listings, including 48 barangay name listings. See `src/data.json` for per-entry sources, review dates and caveats. Contact numbers have not been telephone-tested. Sources reviewed 8–9 November 2026; individual review dates are preserved. Barangay listings are names only, not verified contact listings. Historical procurement records do not establish delivery or completion. Added BLGF FY2025 preliminary reported actuals with clear units and provenance; no FY2026 appropriation, audited spending or complete recent ordinance archive is claimed.

## Contribute

Open an issue or PR with a public source for corrections. Add the source URL, `reviewed` date, and a note explaining uncertainty. Rebuild and check search, all six sections, dialogs, CSV and mobile before publishing. Review public sources quarterly; no automatic monitoring is configured.

## Deployment

Live site: https://bettertanauanbatangas.vercel.app/

Vercel builds the `main` branch with `node build.mjs` and publishes `dist/`. This repository contains no hosting credentials or inherited Sites project ID. See `BETTERGOV-SUBMISSION.md` for a draft registration row. Do not claim Active while the public portal is not live.

## Sources

- https://fdpp.blgs.gov.ph/
- https://gad.tanauancity.gov.ph/
- https://notices.philgeps.gov.ph/GEPSNONPILOT/Tender/PrintableBidNoticeAbstractUI.aspx?refid=12413893
- https://psa.gov.ph/classification/psgc/barangays/0401031000
- https://sample1.tanauancity.gov.ph/wp-content/uploads/2020/07/Annual-Budget-Report-2023.pdf
- https://tanauancity.gov.ph/
- https://tanauancity.gov.ph/admin/wp-content/uploads/2025/02/City-Ordinance-2014-29-1.pdf
- https://tanauancity.gov.ph/government/citizens-charter
- https://tanauancity.gov.ph/government/departments/mayors-office
- https://tanauancity.gov.ph/news/-2025-

## Template
[BetterSolano](https://github.com/BetterSolano/bettersolano), static main branch, adapted with attribution. See TEMPLATE.md for the pinned commit and exact changes. The existing LGU data and Git history are preserved.
