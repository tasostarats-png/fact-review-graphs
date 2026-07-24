# Fact Review — GitHub Pages graphs

This package contains two standalone, build-free graphs:

- `timeline/index.html` — posting timeline
- `profile-carousel/index.html` — two-row profile-picture carousel

## Upload to GitHub

1. Create a repository, for example `fact-review-graphs`.
2. Upload the complete `timeline` and `profile-carousel` folders without
   changing their internal structure.
3. In GitHub, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the `main` branch and `/ (root)`, then save.

The public addresses will be:

- `https://USERNAME.github.io/fact-review-graphs/timeline/`
- `https://USERNAME.github.io/fact-review-graphs/profile-carousel/`

Replace `USERNAME` and `fact-review-graphs` with the actual GitHub username and
repository name.

## WordPress iframe

Add each graph in a WordPress **Custom HTML** block:

```html
<iframe
  src="GITHUB_PAGES_URL"
  title="Graph title"
  width="100%"
  height="850"
  loading="lazy"
  style="display:block;width:100%;height:850px;border:0;"
></iframe>
```

For the profile carousel, keep the `profiles` folder next to its `index.html`;
otherwise its portrait images will not load.
