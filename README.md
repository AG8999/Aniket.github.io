# Aniket Ghadge — Portfolio

Jekyll-based personal portfolio. Hosted via GitHub Pages with custom domain support.

## Local Development

```bash
gem install bundler
bundle install
bundle exec jekyll serve
# Open http://localhost:4000
```

## Deploy to GitHub Pages (Custom Domain)

1. Create a repo named `your-username.github.io` on GitHub
2. Push this folder to that repo
3. Go to **Settings → Pages** → set source to `main` branch
4. In **Settings → Pages → Custom domain**, enter your domain (e.g. `aniketghadge.dev`)
5. Update `CNAME` file with your domain
6. At your domain registrar, add DNS records:
   - `A` records pointing to GitHub Pages IPs:
     - `185.199.108.153`
     - `185.199.109.153`
     - `185.199.110.153`
     - `185.199.111.153`
   - `CNAME` record: `www` → `your-username.github.io`
7. Update `url` in `_config.yml` to your custom domain

DNS propagation takes ~24–48 hours. GitHub will auto-provision HTTPS via Let's Encrypt.

## Customisation

- **Content**: Edit `index.html` directly
- **Styles**: Edit `assets/css/main.css`
- **Config**: Edit `_config.yml` for site metadata
- **Custom domain**: Edit `CNAME`
