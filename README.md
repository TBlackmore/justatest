# Astro Starter Kit: Blog

[![Deploy to Cloudflare](https://deploy.workers.cloudflare.com/button)](https://deploy.workers.cloudflare.com/?url=https://github.com/cloudflare/templates/tree/main/astro-blog-starter-template)

![Astro Template Preview](https://github.com/withastro/astro/assets/2244813/ff10799f-a816-4703-b967-c78997e8323d)

<!-- dash-content-start -->

Create a blog with Astro and deploy it on Cloudflare Workers as a [static website](https://developers.cloudflare.com/workers/static-assets/).

Features:

- ✅ Minimal styling (make it your own!)
- ✅ 100/100 Lighthouse performance
- ✅ SEO-friendly with canonical URLs and OpenGraph data
- ✅ Sitemap support
- ✅ RSS Feed support
- ✅ Markdown & MDX support
- ✅ Built-in Observability logging

<!-- dash-content-end -->

## Getting Started

Outside of this repo, you can start a new project with this template using [C3](https://developers.cloudflare.com/pages/get-started/c3/) (the `create-cloudflare` CLI):

```bash
npm create cloudflare@latest -- --template=cloudflare/templates/astro-blog-starter-template
```

A live public deployment of this template is available at [https://astro-blog-starter-template.templates.workers.dev](https://astro-blog-starter-template.templates.workers.dev)

## 🚀 Project Structure

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.

There's nothing special about `src/components/`, but that's where we like to put any Astro/React/Vue/Svelte/Preact components.

The `src/content/` directory contains "collections" of related Markdown and MDX documents. Use `getCollection()` to retrieve posts from `src/content/blog/`, and type-check your frontmatter using an optional schema. See [Astro's Content Collections docs](https://docs.astro.build/en/guides/content-collections/) to learn more.

Any static assets, like images, can be placed in the `public/` directory.

### Community Blog Structure

In addition to the Astro blog, this repository includes a separate community blog structure:

```plaintext
justatest/
├── blog/
│   ├── assets/
│   │   └── placeholder-image.jpg    # Placeholder images and assets
│   └── posts/
│       └── sample-post.md            # Community blog posts
├── src/
│   └── main.py                       # Python backend for community blog
```

**Community Blog Features:**
- `blog/posts/` - Markdown files for community blog posts
- `blog/assets/` - Image assets and media files
- `src/main.py` - Python application for processing blog content

To run the community blog Python application:
```bash
python3 src/main.py
```

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

### Astro Blog Commands

| Command                           | Action                                           |
| :-------------------------------- | :----------------------------------------------- |
| `npm install`                     | Installs dependencies                            |
| `npm run dev`                     | Starts local dev server at `localhost:4321`      |
| `npm run build`                   | Build your production site to `./dist/`          |
| `npm run preview`                 | Preview your build locally, before deploying     |
| `npm run astro ...`               | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help`         | Get help using the Astro CLI                     |
| `npm run build && npm run deploy` | Deploy your production site to Cloudflare        |
| `npm wrangler tail`               | View real-time logs for all Workers              |

### Community Blog Commands

| Command                    | Action                                      |
| :------------------------- | :------------------------------------------ |
| `python3 src/main.py`      | Run the community blog Python application   |

### Development Instructions

**For the Community Blog:**

1. **Adding New Blog Posts:**
   - Create a new `.md` file in `blog/posts/`
   - Use `blog/posts/sample-post.md` as a template
   - Include front matter with title, date, author, and tags

2. **Adding Assets:**
   - Place images and media files in `blog/assets/`
   - Reference them in posts using relative paths: `../assets/your-image.jpg`

3. **Extending Python Backend:**
   - Edit `src/main.py` to add new functionality
   - The `CommunityBlog` class provides methods for listing posts and assets
   - Extend with markdown parsing, rendering, or API endpoints as needed

## 👀 Want to learn more?

Check out [our documentation](https://docs.astro.build) or jump into our [Discord server](https://astro.build/chat).

## Credit

This theme is based off of the lovely [Bear Blog](https://github.com/HermanMartinus/bearblog/).
