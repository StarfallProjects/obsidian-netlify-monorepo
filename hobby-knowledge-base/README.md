# hobby-knowledge-base README

This site is part of a larger example project, showing how to deploy multiple websites from one [Obsidian](https://obsidian.md/) vault, using a [GitHub](https://github.com/) monorepo and [Netlify](https://www.netlify.com/). To learn more about this deployment setup, [refer to the tutorial](https://www.starfallprojects.co.uk/posts/obsidian-monorepo/).

The site uses [MkDocs](https://www.mkdocs.org/) and the [Material](https://squidfunk.github.io/mkdocs-material/getting-started/) theme to create a knowledge base. It uses minimal configuration and demo content. This README gives some additional information, which may be helpful if you want to actually use this example site.

## Run locally - quickstart

You will need [Python 3](https://www.python.org/downloads/) installed on your machine.

1. Clone the repo:
    ```
    git clone https://github.com/StarfallProjects/obsidian-netlify-monorepo.git
    ```
2. Navigate into `hobby-knowledge-base`:
    ```
    cd /path/to/hobby-knowledge-base
    ```
3. Recommended: create a virtual environment using venv:
    ```
    python -m venv venv
    ```
    If you call your venv something other than 'venv', make sure to update the `.gitignore` file.
4. Install MkDocs and Material:
    ```
    pip install requirements.txt
    ```
5. Run MkDocs locally:
    ```
    mkdocs serve
    ```
6. View the site at `localhost:8000`.

## Wikilinks

Obsidian supports wikilinks. These are links between files created using double square brackets: `[[link]]`. This differs from the standard markdown link syntax:

```
[link title](link url)
```

I've used the [Python Markdown wikilinks extension](https://python-markdown.github.io/extensions/wikilinks/) to add support for wikilinks.

This is done in the `mkdocs.yml` config file:

```
markdown_extensions:
  - wikilinks
```


