# Jamie Hamilton portfolio

Static site served by Cloudflare Workers static assets. No build step.

```
wrangler.jsonc      tells Cloudflare to serve ./public
public/index.html   the site
public/_headers     security headers
```

## Deploy (Cloudflare, connected to this GitHub repo)

1. Cloudflare dashboard, Workers & Pages, Create application, Import a repository
2. Pick this repo
3. Build command: leave blank
4. Deploy command: `npx wrangler deploy` (the default)
5. Save and Deploy

Every push to `main` redeploys. Custom domain: the Worker's Settings, Domains & Routes, Add, Custom domain.
