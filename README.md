# SwanLake Website

This repository contains the Hugo + Docsy website for the SwanLake project.

- Main project: <https://github.com/swanlake-io/swanlake>
- Website source: <https://github.com/swanlake-io/swanlake.github.io>

## Local development

Prerequisites:
- Hugo extended (`>= 0.155.0`)
- Go (for Hugo module resolution)

Run locally:

```bash
hugo server
```

Build static output:

```bash
hugo --gc --minify
```

## Content structure

- Homepage: `content/en/_index.md`
- Docs landing: `content/en/docs/_index.md`
- Core docs pages: `content/en/docs/*.md`
- About page: `content/en/about/index.md`
- Community page: `content/en/community/_index.md`
- Static images: `static/images/`

## Deployment

This site is intended for GitHub Pages deployment from this repository.

If you decide between `swanlake.github.io` and `swanlake-io.github.io`, update `baseURL` in `hugo.yaml` to the final canonical URL.
