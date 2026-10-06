# Lingyi Meng's Academic Homepage

Personal academic homepage built with [Hugo](https://gohugo.io/) and based on the [Zero Academic Page](https://github.com/geekifan/zero-academic-page) theme.

## Local development

Install Hugo Extended, then run the following command from the repository root:

```bash
hugo server --source exampleSite --disableFastRender
```

Open <http://localhost:1313/> in a browser. Hugo watches the source files and refreshes the site when they change.

To create a production build locally:

```bash
hugo --source exampleSite --minify --gc
```

The generated website will be written to `exampleSite/public/`.

## Content locations

- English homepage: `exampleSite/content/_index.md`
- English name, sidebar summary, and navigation: `exampleSite/config/_default/languages.toml`
- Shared profile image and social links: `exampleSite/config/_default/params.toml`
- Profile image file: `exampleSite/assets/images/profile.png`

Pushing to `main` triggers the GitHub Actions workflow that builds the Hugo site and publishes it to the `gh-pages` branch.
