# About

This repository contains files for my personal website. The site is written in Emacs using Org Markdown files, which are then converted to HTML using `org-publish`. The main branch includes the Org files in the `org` directory and the CSS file in the `public` directory. The site is automatically generated using the `build-site.el` script, which saves the converted HTML files into the `public` directory with the existing CSS file. The GitHub Actions script in `.github/workflows` will tell GitHub to generate the site and push to `gh-pages` branch when it detects pushes to `main`. The `gh-pages` branch is where the site is deployed from.

## Building the Site Manually

To manually build the site, just clone the repository and run the included `build.sh` script. The generated site will be placed into the `public` directory. 

Here is the command to build:

```bash
$ git clone https://github.com/cbraidwood/website.git && cd website && chmod +x build.sh && ./build.sh
```
