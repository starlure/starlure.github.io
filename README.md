# starlure.github.io

Personal blog built with [Hexo](https://hexo.io/) and the [NeXT](https://theme-next.js.org/) theme.

## Branch layout

- **`source`** (this branch) — the Hexo project source. Edit here.
- **`master`** — generated static HTML served by GitHub Pages. Produced by `hexo deploy`; do not edit by hand.

## Setup

```bash
npm install
```

## Writing

```bash
npx hexo new "My Post Title"   # creates source/_posts/My-Post-Title.md
npx hexo server                # preview at http://localhost:4000
```

Posts live in `source/_posts/*.md`. The About page is `source/about/index.md`.

## Publishing

```bash
npx hexo clean && npx hexo generate   # build into public/
npx hexo deploy                       # force-push public/ to master
git add -A && git commit -m "..."     # save the source
git push origin source
```

## Configuration

- `_config.yml` — site config (title, author, URL, deploy target).
- `_config.next.yml` — NeXT theme config (menu, social links, scheme).
