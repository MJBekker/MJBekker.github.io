---
title: GitHub Pages
tags: GitHub
---

Setting up a GitHub page is awesome an free! Read more to find out how to set up.

<!--more-->

---

# GitHub Pages: A Brief Introduction

GitHub Pages is a static site hosting service provided by GitHub. It allows you to create and publish webpages directly from your GitHub repository. Here's a brief overview:

## What is GitHub Pages?

- GitHub Pages takes HTML, CSS, and JavaScript files from a repository on GitHub, optionally runs them through a build process, and publishes a website.
- You can use GitHub Pages to showcase open source projects, host a blog, or even share your résumé.

## Getting Started

1. **Create a Repository:**
   - In the upper-right corner of any page on GitHub, click the "+" button and select "New repository."
   - Name your repository as `username.github.io`, replacing `username` with your GitHub username (e.g., if your username is "octocat," the repository name should be "octocat.github.io").

2. **Configure GitHub Pages:**
   - Under your repository settings, navigate to the "Pages" section.
   - Choose a publishing source (usually the "main" branch) and optionally edit the README.md file to add content for your site.
   - Visit `username.github.io` (replace `username` with your actual GitHub username) to view your new website. Note that it might take up to 10 minutes for changes to publish after pushing them to GitHub.

3. **Customize Your Site:**
   - By default, the title of your site will be `username.github.io`. You can change this by editing the `_config.yml` file in your repository.
   - To modify the title and description:
     - Go to the "Code" tab of your repository.
     - Open the `_config.yml` file.
     - Add lines for `title` and `description` (e.g., `title: My Awesome Site` and `description: A place for my projects`).
     - Commit your changes.

## Next Steps

Great! You have set up your own website with the help of GitHub pages. But are you feeling underwhelmed with the basic
text basted website. Are you looking to make it prettier and more blog like? The easiest starting point is to use a
[jekyll-template](https://github.com/topics/jekyll-template). To set up the popular
[jekyll-TeXt-theme](https://github.com/kitian616/jekyll-TeXt-theme) read the next section.

## jekyll-TeXt-theme

This theme can enhance your experience with GitHub Pages a lot and it is easy to set up. If you have an existing GitHub Pages repository set up, simply clone the theme repository and copy over the files:
```bash
USERNAME=<username>
git clone https://github.com/${USERNAME}/${USERNAME}.github.io.git
git clone https://github.com/kitian616/jekyll-TeXt-theme.git
cp -r jekyll-TeXt-theme/* ${USERNAME}.github.io
cd ${USERNAME}.github.io
git stage .
git commit -m 'Adopting jekyll-TeXt-theme theme'
git push
```
