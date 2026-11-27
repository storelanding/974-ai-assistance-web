# Ai assistance — website

Static landing site for the **Ai assistance** Android app on Google Play
(`com.ai.assistant.smart.chat.helper`). Plain HTML + CSS, no build step.

| File | Purpose |
| --- | --- |
| `index.html` | App landing page |
| `policies.html` | Privacy Policy (use this URL on the store listing) |
| `terms.html` | Terms of Use |
| `app-ads.txt` | Authorized ad sellers file |
| `404.html` | Not-found page |
| `assets/` | `style.css`, `icon.svg`, images in `assets/img/` |
| `site.json` | Metadata the site was generated from |

## Deploy

**Cloudflare Pages:** Workers & Pages → Create → Pages → Connect to Git → choose this repo.
Framework preset **None**, build command empty, output directory `/`. Add your domain under Custom domains.

**Vercel:** Add New → Project → import this repo. Framework **Other**, no build command,
output directory `.`. Add your domain under Settings → Domains.

## After deploying

- `app-ads.txt` must be reachable at `https://<your-domain>/app-ads.txt`, and that domain must match the
  developer website declared on Google Play.
- Privacy Policy URL for the store listing: `https://<your-domain>/policies.html`.
