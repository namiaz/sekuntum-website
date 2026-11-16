# Sekuntum Photobooth website

Marketing site for https://sekuntum.my (static HTML, no build step).

```
site/     what gets published (index.html + assets/)
docs/     planning notes, never published
design/   design notes; large originals are kept out of git
```

## Deploy
Cloudflare Pages / Workers, connected to this repo:
- Build command: none
- Output directory: `site`
- Production branch: `main`

## Working on a change
1. `git switch -c my-change`
2. Edit files in `site/`, preview with `python3 -m http.server 8766 --directory site`
3. Push the branch; Cloudflare builds a preview link
4. Merge to `main` to publish

## Related (separate repos, later)
- `sekuntum-magnet` → magnet.sekuntum.my
- `sekuntum-admin` → admin.sekuntum.my

Never commit passwords, API keys or tokens.
