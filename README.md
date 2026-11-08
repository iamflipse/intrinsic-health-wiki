# Intrinsic Health Wiki

A curated wiki distilling:

> Cohen AA (2026). "Intrinsic Health: A New Way to Understand How Our Bodies Maintain Their Internal Balance." *The Science and Experience of Energy* (Martin Picard, Substack), Mar 2026. https://tseenergy.substack.com/p/intrinsic-health-a-new-way-to-understand
> Related paper: Cohen, Picard et al., *Science Advances* (2025) — the intrinsic/realized health framework.

**Public copy:** https://iamflipse.github.io/intrinsic-health-wiki/ (read-only; static build served from the `gh-pages` branch)

## Layout

- `src/` — wiki pages as markdown (`index.md`, `about.md`, `concepts/`, `sources/`)
- `book/` — mdbook-generated static site (committed for GitHub Pages)
- `tools/mdbook` — mdbook v0.4.21 binary (aarch64 Linux, built from source)

## Rebuild + republish

```sh
./tools/mdbook build -d book
git add -A && git commit -m "update" && git push origin main
# republish gh-pages: check out orphan branch, copy book/* to root, add .nojekyll, force push
```
