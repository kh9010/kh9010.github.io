# kh9010.github.io — the preview of kahransingh.com

This repo holds no pages of its own. Its one workflow fetches the `preview`
branch of [kh9010/kahransingh.com](https://github.com/kh9010/kahransingh.com)
and publishes it to GitHub Pages at https://kh9010.github.io/.

- **Live** = `main` of kahransingh.com → https://kahransingh.com (that repo's own Pages).
- **Preview** = `preview` of kahransingh.com → https://kh9010.github.io/ (this repo).

To put a branch on preview, from the kahransingh.com checkout: `tools/preview.sh [branch]`
(pushes the branch to `preview` and dispatches the workflow here). The workflow also
runs every 30 minutes, so a plain `git push origin <branch>:preview` lands within half an hour.

The preview copy drops the `CNAME` file and ships a `robots.txt` that disallows everything,
so it never competes with the live site in search. No secrets: the source repo is public.
