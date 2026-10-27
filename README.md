# kh9010.github.io — the preview of kahransingh.com

This repo holds no pages of its own. Its `main` is a copy of the `preview` branch of
[kh9010/kahransingh.com](https://github.com/kh9010/kahransingh.com), pushed here by a
scheduled job on Kahran's Mac mini (`tools/preview-publish.sh` in that repo), and served by
GitHub Pages at https://kh9010.github.io/.

- **Live** = `main` of kahransingh.com → https://kahransingh.com (that repo's own Pages).
- **Preview** = `preview` of kahransingh.com → https://kh9010.github.io/ (this repo).

To put a branch on preview, from the kahransingh.com checkout: `tools/preview.sh [branch]`.
The copy drops `CNAME` and ships a `robots.txt` that disallows everything, so it never competes
with the live site in search. Do not edit this repo by hand; the next publish overwrites it.
