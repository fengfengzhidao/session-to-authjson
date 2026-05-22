# session-to-authjson

A static HTML converter for turning a ChatGPT session JSON export into an auth JSON shape.

Open [index.html](./index.html) in a browser, paste the source JSON, and convert it locally. The page does not send tokens anywhere and does not store them in local storage.

## GitHub Pages

This repository publishes the static page from the `gh-pages` branch.

In repository **Settings -> Pages**, choose:

- Source: `Deploy from a branch`
- Branch: `gh-pages`
- Folder: `/ (root)`

After GitHub finishes deployment, the site will be available at:

```text
https://<your-user-name>.github.io/<repository-name>/
```
