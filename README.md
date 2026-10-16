# Pathway — demand-test landing page

Static site, single `index.html`. Hosted on GitHub Pages.

- Signups POST as JSON to Formspree (`CONFIG.endpoint` in `index.html`). Two record types arrive: `signup` and `survey`, joined by `id`.
- Analytics: paste a Plausible or GA4 snippet into `<head>`; `track()` fires `page_view`, `goal_typed`, `cta_find_routes`, `example_goal`, `plan_interest`, `signup`, `survey_complete`, `share_copy` with UTM and referrer.
- Custom domain: add a `CNAME` file with the domain and point DNS at GitHub Pages.
