# Anvita privacy and support website

A buildless GitHub Pages website for Anvita, operated by **flexiorder**. Public support: **flexiorderofficial@gmail.com**.

## Pages

- `/` — privacy and support home
- `/privacy/` — privacy policy
- `/delete-account/` — external account-deletion request instructions
- `/contact/` — app support and privacy contact
- `/terms/` — terms of use

All internal paths are relative, so the site works at `https://ishwrknt.github.io/heartsync-legal/` as well as under a custom domain. Only static HTML, CSS and the existing Anvita SVG icon are needed. No build or runtime dependencies, forms, analytics scripts, public app configuration or account credentials are included.

## Preview

From this directory:

```bash
python3 -m http.server 4178 --bind 127.0.0.1
```

Then visit `http://127.0.0.1:4178/`. To check project-prefix behavior, serve its parent `sites/` directory and visit `/heartsync-legal/`.

## Publish

Publish only this directory as a separate repository. GitHub Pages can serve the root of its `main` branch; `.nojekyll` disables unnecessary Jekyll processing. The GitHub account must be authorized to publish the repository. The working app and its private configuration do not belong in this public repository.

After publication verify all five direct HTTPS page URLs, internal links, stylesheet/icon paths, and the account-deletion email draft in an actual mail client. Opening an email link does not submit or send a request.

## Play Console links after publication

Expected URLs, which must be checked live before submission:

- Privacy: `https://ishwrknt.github.io/heartsync-legal/privacy/`
- Account deletion: `https://ishwrknt.github.io/heartsync-legal/delete-account/`
- Website: `https://ishwrknt.github.io/heartsync-legal/`
- Contact: `https://ishwrknt.github.io/heartsync-legal/contact/`

Source references: the application's `docs/PRIVACY.md`, `store/DATA_SAFETY_DRAFT.md`, `src/components/PublicPage.tsx` and current native companion lifecycle implementation. Current Play guidance permits a customer-service email as the web deletion request pathway: <https://support.google.com/googleplay/android-developer/answer/13327111>.

## Operational responsibilities

The publisher must monitor the support inbox, verify account ownership proportionately, complete deletion requests, confirm outcomes and maintain consistency between the app, policy and Play Data safety declarations. The pages intentionally publish no unconfirmed 30-day request SLA, fixed backup-erasure deadline, hosting region or assertion that a scheduled purge is already running. Confirm actual retention, purge operation and provider backup settings before a public app rollout; update the policy with verified details where appropriate.

This site provides an email pathway, not an authenticated deletion backend. It does not verify that hosted account-deletion migrations or administrator procedures are deployed. A live page alone does not establish Play approval or production release readiness. Recheck the published copy whenever features or data practices change.
