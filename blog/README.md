# blog README

This site is part of a larger example project, showing how to deploy multiple websites from one [Obsidian](https://obsidian.md/) vault, using a [GitHub](https://github.com/) monorepo and [Netlify](https://www.netlify.com/). To learn more about this deployment setup, [refer to the tutorial](https://www.starfallprojects.co.uk/posts/obsidian-monorepo/).

The site uses [Eleventy](https://www.11ty.dev/) and the [Eleventy Base Blog](https://github.com/11ty/eleventy-base-blog) starter to create a blog. It uses minimal configuration and demo content. This README gives some additional information, which may be helpful if you want to actually use this example site.

## Run locally - quickstart

You will need [Node.js](https://nodejs.org/en/) installed on your machine.

1. Clone the repo:
    ```
    git clone https://github.com/StarfallProjects/obsidian-netlify-monorepo.git
    ```
2. Navigate into `blog`:
    ```
    cd /path/to/blog
    ```
3. Install dependencies:
    ```
    npm install
    ```
4. Run Eleventy locally:
    ```
    npx eleventy --serve
    ```
5. View your site at `localhost:8080`.

## Wikilinks

Obsidian supports wikilinks. These are links between files created using double square brackets: `[[link]]`. This differs from the standard markdown link syntax:

```
[link title](link url)
```

Eleventy does not support these by default. There are various plugins available that extend [markdown-it](https://github.com/markdown-it/markdown-it) to have wikilink support. Alternatively, you can use standard markdown links in Obsidian, or use [Wikilinks to MDLinks])(https://github.com/agathauy/wikilinks-to-mdlinks-obsidian) to convert links within Obsidian.
