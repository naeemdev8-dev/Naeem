# Portfolio site SOPs

Single-page portfolio for Naeem Ashraf: `index.html` plus media in `videos/` and `samples/`, and the owner's photo in `images/`. The video grid is built from `videos.json`, which the owner manages through `admin.html`. Hosted on GitHub Pages from `main` at https://naeemdev8-dev.github.io/Naeem/. The repo is public.

Follow these on every update.

## Content rules

1. **One brand only.** Daiichi Technologies is the only brand or company shown.
2. **No client names.** The one exception is the testimonial in rule 3.
3. **One testimonial only.** Muhammad Nadeem, Daiichi Technologies. The spelling is "Nadeem", never "Naeem". Naeem Ashraf is the site owner, a different person.
4. **Nothing invented.** Do not write or add reviews, star ratings, results, numbers or client names unless the owner supplies them and approves them.
5. **Rules 1 and 2 cover everything public**, not just visible text: page text, captions, `<title>`, meta and `og:` tags, `aria-label`s, alt text, file names, commit messages, and this file and `README.md`. Do not name removed clients here, even to ban them.

## Before every commit

1. Run `git pull`. Uploads from `admin.html` commit directly to `main`, so the local copy may be behind.
2. Read the changed text against the content rules, including anything new in `videos.json`.
3. Run `git status` and confirm only intended files are staged.
4. Confirm every `src`, `poster`, `file` and `poster` path in `index.html` and `videos.json` points to a tracked file, using a relative path and matching upper and lower case. GitHub Pages is case-sensitive and serves from `/Naeem/`.
5. `.gitignore` allows only `videos/daiichi-technologies.*` from `videos/`. Do not widen it or force-add other media from there without the owner's approval.

## Sample uploads

1. New videos and images go in `samples/` with generated names (`sample-<timestamp>`), because original file names may name a client. `admin.html` does this, so keep it if you change that page.
2. Commit messages from `admin.html` stay generic and never include sample titles.
3. `admin.html` holds no credentials. The owner's token stays in their browser. Never commit a token, and do not add third-party scripts or styles to that page.

## Publishing

1. Commit to `main` with a message that names no clients, then push.
2. Do not force-push or rewrite history without the owner's explicit approval.
3. Check the live URL and report what actually loaded. If Pages is not serving the change yet, say so.
