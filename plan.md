# Setup
-------------------------

## Personal page (`<username>.github.io`)

### 1. Fork the repository
Fork the repository from [here](https://github.com/kbsezginel/gh-pages-template) by clicking the fork button on the top right corner.

### 2. Rename the repository
Go to `Settings -> Repository name` and write down `<username>.github.io`.

## Project page (`<username>.github.io/<myproject>`)

### 1. Fork the repository
Fork the repository from [here](https://github.com/kbsezginel/gh-pages-template) by clicking the fork button on the top right corner.

### 2. Enable GitHub Pages
Go to `Settings -> GitHub Pages` in your fork of the repository.
Under `source` select `master branch`.

# Customization
-------------------------

## Configuring the site
Edit the `_config.yml` file and change the site title and description.
Remove the `setup.md` file (optional).

## Adding pages
To add a new page you need to create a new markdown file with the name of your choice.
For example here `setup.md` file is used to generate content for the `setup` page.

### Layouts
There are currently two layouts: `default` and `full`.
In the `default` layout a sidebar containing navigation is present whereas in `full` layout the full page is reserved for page content.
The `full` layout can be selected by adding a yaml front matter to the markdown/html file:
```
---
layout: full
---
```


# 回顧與計畫
-------------------------

- [Minimal theme GitHub repository](https://github.com/pages-themes/minimal)

More tutorials on github pages, markdown and Jekyll can be found here:
- Review 目前項目
- 定2021基礎版規格及開發計畫
