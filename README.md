# Medium Card Widget

A dynamic card widget that generates beautiful preview images for Medium articles. Perfect for GitHub READMEs, portfolios, and documentation.

![Example Card](https://medium-card-widget.vercel.app/api/card?url=https://medium.com/@ojasvissar/ai-in-the-fight-against-climate-change-predicting-environmental-trends-before-its-too-late-0ca6fadce36f)

## Usage

### Basic Usage

Simply replace `YOUR_MEDIUM_ARTICLE_URL` with your Medium article link:

```
https://medium-card-widget.vercel.app/api/card?url=YOUR_MEDIUM_ARTICLE_URL
```

### In GitHub README (Markdown)

```markdown
[![Medium Article](https://medium-card-widget.vercel.app/api/card?url=YOUR_MEDIUM_ARTICLE_URL)](YOUR_MEDIUM_ARTICLE_URL)
```

### In GitHub README (HTML - Recommended for sizing)

```html
<a href="YOUR_MEDIUM_ARTICLE_URL">
  <img src="https://medium-card-widget.vercel.app/api/card?url=YOUR_MEDIUM_ARTICLE_URL" width="600" alt="Medium Article" />
</a>
```

### Example

For an article at `https://medium.com/@username/my-article-title-abc123`:

```markdown
[![My Article](https://medium-card-widget.vercel.app/api/card?url=https://medium.com/@username/my-article-title-abc123)](https://medium.com/@username/my-article-title-abc123)
```

## Features

- **Dynamic metadata extraction** - Automatically fetches title, description, and cover image
- **High-resolution output** - 1600x560px for crisp rendering on all displays
- **GitHub-style dark theme** - Matches GitHub's dark mode aesthetic
- **Horizontal layout** - Image on left, content on right
- **Click-through support** - Links directly to your Medium article

## Important Notes

1. **URL Encoding**: If your Medium URL contains special characters, you may need to URL-encode it
2. **Caching**: Images are cached by Vercel's CDN. Changes to your article may take some time to reflect
3. **Rate Limits**: This uses the free tier of microlink.io API for metadata extraction

## Self-Hosting

Want to host your own instance? Fork this repo and deploy to Vercel:

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/ojasvissar/medium-card-widget)

## Tech Stack

- [Vercel Edge Functions](https://vercel.com/docs/functions/edge-functions)
- [@vercel/og](https://vercel.com/docs/functions/og-image-generation) - Image generation
- [Microlink API](https://microlink.io/) - Metadata extraction

## License

MIT

---

Made with ❤️ by [@ojasvissar](https://github.com/ojasvissar)
