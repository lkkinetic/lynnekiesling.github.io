# lynnekiesling.com

Source for Lynne Kiesling's personal site, built with Jekyll and hosted on
GitHub Pages. Replaces the previous WordPress/Elementor site.

## Structure

- `index.md` — home/bio, current & past appointments, education, contact
- `publications.md` — books, edited volumes, chapters, articles, working
  papers/current projects, grants
- `leadership.md` — workshops directed, professional leadership/convening
- `teaching.md` — teaching, policy reports, op-eds, past advisory roles
- `cv.md` — on-site CV summary + link to downloadable PDF
- `_data/*.yml` — all list content (publications, workshops, leadership
  roles, etc.) lives here as data, not hardcoded in the page templates.
  **To add a new publication, workshop, role, etc., edit the relevant
  YAML file in `_data/` — you don't need to touch any HTML/Markdown.**
- `_layouts/`, `_includes/`, `assets/css/` — site theme (custom,
  Hyde-inspired sidebar layout)

## Known TODOs before/after first deploy

- `assets/cv/Kiesling_CV.pdf` — placeholder only. Drop in the real CV PDF
  export (see `assets/cv/README.md`).
- `_config.yml` — `linkedin` and `youtube` fields are placeholders
  (`TODO-LINKEDIN-URL` / `TODO-YOUTUBE-URL`). Fill in your actual profile
  and channel URLs.
- `_data/books.yml` — `chapters:` list is empty; CV lists 7 book chapters
  (2014–2021) not individually itemized in the redesign spec.
- `_data/policy_reports.yml` — only 1 of ~7 CV-listed policy reports is
  itemized.
- `_data/op_eds.yml` — only outlet names given, not individual titles/dates.

## Local preview

```bash
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000.

## Custom domain (lynnekiesling.com) via Network Solutions

The `CNAME` file in this repo already contains `lynnekiesling.com`. Once
this repo is pushed to GitHub as `lkkinetic/lynnekiesling.github.io` and
Pages is enabled:

1. Log into Network Solutions → find `lynnekiesling.com` → Manage DNS /
   Advanced DNS Records.
2. For the apex domain (`lynnekiesling.com`), remove any A records
   pointing at the old WordPress host and add these four A records
   pointing to GitHub Pages:
   - `185.199.108.153`
   - `185.199.109.153`
   - `185.199.110.153`
   - `185.199.111.153`
   (Optional AAAA records for IPv6: `2606:50c0:8000::153`,
   `2606:50c0:8001::153`, `2606:50c0:8002::153`, `2606:50c0:8003::153`.)
3. For `www`, add/update a CNAME record: `www` → `lynnekiesling.github.io`.
4. In the GitHub repo's Settings → Pages, enter the custom domain
   (`lynnekiesling.com`) and wait for the DNS check to pass, then enable
   **Enforce HTTPS**.
5. DNS propagation is typically a few hours, up to 24–48h. The old
   WordPress site keeps serving until it completes.

## Follow-on work (not part of this build)

- Migrate the History of Economic Thought video channel from Vimeo to
  this site (likely under Teaching).
- Once `knowledgeproblem.com` is CNAME'd to the Substack, update the
  footer/nav links from `knowledgeproblem.substack.com` to
  `knowledgeproblem.com`.
