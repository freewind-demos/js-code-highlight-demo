Highlight.js Demo
=================

Use [highlight.js](https://github.com/highlightjs/highlight.js) to highlight code blocks in html.

```
npm install
npx browserify app-all.js > app-all-bundle.js
```

Then open `index.html` in your browser.

Notice
------

We have to use pre-bundled js files from CDN hosts, or do it by ourselves.

See `app-all.js`:

- `hljs.registerLanguage(...)` to include expected language
- `hljs.initHighlightingOnLoad()` to find code blocks in page and render them

And we have to use `browserify` to convert it if we want to use it in html page.