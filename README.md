# Guilherme Passos — Data Engineering Portfolio

A responsive static portfolio covering InMarket audience distribution, Quext Snowflake integrations, Airbnb pipeline recovery, public projects, and engineering practices.

## Preview

From this directory:

```sh
python3 -m http.server 8000 --directory docs
```

Open http://localhost:8000. No build or dependency installation is required. Fonts load from Google Fonts with system-font fallbacks. All other assets are local; there is no tracking, backend, or form submission.

## Publish to GitHub Pages

Publish this directory as the `gpass0s/data-engineering-portfolio` repository. Under **Settings → Pages**, select **Deploy from a branch**, then **main /docs** and save. The expected URL is `https://gpass0s.github.io/data-engineering-portfolio/` once GitHub finishes building. Relative asset paths support both project and account Pages sites.

With authenticated GitHub CLI, from this directory:

```sh
gh repo create gpass0s/data-engineering-portfolio --public --source=. --remote=origin --push
gh api --method POST repos/gpass0s/data-engineering-portfolio/pages -f 'source[branch]=main' -f 'source[path]=/docs'
```

Do not run repository creation if the repository already exists. Check Pages build status and the live URL before sharing it.

## Content and review

- Professional case studies use STAR and distinguish personal contribution from team outcomes.
- Results come from Guilherme’s professional presentation; no numerical improvement claims were invented.
- Architecture diagrams are simplified HTML sequences, not production diagrams.
- Personal-project article images are from the supplied presentation. No private source code, customer data, internal infrastructure identifiers, or raw résumé/presentation files are published.
- Airflow certification links to the credential; SnowPro Core COF-C03 is explicitly preparation in progress.
- `private/` is excluded from Git. It contains the recruiter reply and local review artifacts. Only `docs/` is served by Pages.

Check the page at mobile and desktop sizes, follow navigation and external links, and inspect the final diff before publishing changes.
