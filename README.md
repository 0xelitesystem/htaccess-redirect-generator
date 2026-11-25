# htaccess Redirect Generator

Build Apache `.htaccess` redirect and rewrite rules in your browser. No server, no tracking, no third-party scripts.

**Live demo:** https://0xelitesystem.github.io/htaccess-redirect-generator/

## Use

Open `index.html` in any modern browser, or visit the GitHub Pages link in the repo description.

Toggle what you need and the snippet updates live:

- Force HTTPS (redirect http to https)
- Normalize www: www to non-www, or the reverse
- Path redirects: 301 or 302, from an old site path to a new path or full URL
- Custom RewriteRules: your own regex pattern and target, as an internal rewrite or an external 301

Click Copy .htaccess to grab the whole snippet. Drop it into the `.htaccess` file at your site root.

Empty and invalid rows are reported inline (missing path, missing target, a full URL where a path is expected).

## Why this exists

Writing `.htaccess` rewrite rules by hand is error-prone, and most online generators bury the output under ads or send your input to a server. This is a single file that builds correct mod_rewrite rules offline.

## Privacy

Everything runs in your browser. Your paths and rules never leave your machine. There are no network requests, no analytics, and no external scripts. Verify by viewing the page source or watching the network tab in DevTools.

## Run locally

```bash
git clone https://github.com/0xelitesystem/htaccess-redirect-generator
cd htaccess-redirect-generator
# Open index.html in your browser, or:
python -m http.server 8000
```

## Build

There is no build. It is a single HTML file.

## More

Part of a catalog of single-file browser tools and plain-language references, all MIT licensed and dependency-free: [0xelitesystem.github.io](https://0xelitesystem.github.io/). Built by [elitesystem.ai](https://elitesystem.ai).

## License

MIT.

## Related

- [browser-fake-test-data](https://github.com/0xelitesystem/browser-fake-test-data)
- [lorem-filler-text-browser](https://github.com/0xelitesystem/lorem-filler-text-browser)
- [jwt-verify-in-browser](https://github.com/0xelitesystem/jwt-verify-in-browser)
