# Ukrainian Alphabet HTML Activity for Wix

This folder is a standalone HTML version of the original SCORM package.

## Files
- `index.html` - the interactive alphabet activity
- `audio/` - pronunciation and quiz sound files

## What changed
- Removed SCORM manifest and SCORM API wrapper.
- Progress is saved locally in the learner's browser using localStorage.
- Added optional `postMessage` events for future custom tracking or iframe height handling.

## How to use in Wix
1. Upload this whole folder to a web host such as Netlify, GitHub Pages, Cloudflare Pages, or your own server.
2. Copy the public HTTPS URL to `index.html`.
3. In Wix, add: Embed Code -> Embed a Site / HTML iframe.
4. Paste the public URL.

Example iframe code:

```html
<iframe
  src="https://your-site.example/ukrainian-alphabet/index.html"
  width="100%"
  height="900"
  style="border:0; border-radius:16px; overflow:hidden;"
  allow="autoplay"
  loading="lazy">
</iframe>
```

## Note
Wix will display this as an embedded interactive activity. It will not collect SCORM reports unless you add custom tracking later with Wix/Velo or use a SCORM host.
