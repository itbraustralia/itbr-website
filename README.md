# IT.BR Australia — Jekyll Site

## Hosting on GitHub Pages

### Setup (one-time)

1. **Push this repo to GitHub** as `itbraustralia/itbraustralia.github.io` (or any repo name)

2. **Enable GitHub Pages** in the repo:
   - Go to **Settings → Pages**
   - Under *Source*, select **GitHub Actions**

3. **Push to `main`** — the Actions workflow will build and deploy automatically.

### Custom domain (itbr.com.au)

The `CNAME` file already contains `itbr.com.au`.

In your DNS provider, add:
```
Type: A
Name: @
Values:
  185.199.108.153
  185.199.109.153
  185.199.110.153
  185.199.111.153

Type: CNAME
Name: www
Value: itbraustralia.github.io
```

Then in GitHub: **Settings → Pages → Custom domain** → enter `itbr.com.au` and enable **Enforce HTTPS**.

### Local development

```bash
bundle install
bundle exec jekyll serve
```

Open http://localhost:4000
