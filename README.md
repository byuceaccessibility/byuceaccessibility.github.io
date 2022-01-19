# BYU CE Accessibility

[![Open in Visual Studio Code](https://img.shields.io/badge/Open%20in-Visal%20Studio%20Code-blue?style=for-the-badge&logo=visualstudiocode)](https://open.vscode.dev/byuceaccessibility/byuceaccessibility.github.io)

Accessibility Help page for BYU CE employees.

# Getting Started

# Adding a Help Page

Adding a help page is very simple. It only requires knowlegdge on the use of a markdown file. If you don't know what 'markdown' is, markdown is a simplified html file. For examples and a how to write in 'markdown' see [Docs Markdown reference](https://docs.microsoft.com/en-us/contribute/markdown-reference) from Microsoft.

## A File to Folder Structure

To start make a new file in the `help\` folder of this respository. Title it using the markdown file exenstion (`YOUR-TITLE.md`). In that file is where we will put all of the content of your new help page.

Copy the text in the next paragraph to your new files contents. This will be the basis we will start the page with.

```markdown
---
layout: page
title: YOUR-PAGE-TITLE
permalink: /help/YOUR-PAGE-TITLE/
---

Your page content...
```

In the prior example code you will see data between lines of hyphens, `---`, and `Your page content...`. The data between the lines of hypens are values that will fill in the basic webpage layout out and make your page match the rest of the website. `Your page content...` is simply filler text that you can replace with markdown of your choice.

## Add the File to Webpage Navigation

Now that you've added the file to our repository, we need to add your page to the basic navigation of the website so people can access it. To do this we will add the title and path to the `_config.yml` file in the base folder of this directory.

Open `_config.yml` and find the portion of code in block below.
```yml
# Navigation
navbar-links:
  About: "/about/"
  Accessibility Panel: "/AccessibilityPanel/"
  Helpful Links:
```
Under `Helpful Links` you will find more code below like `    - Color: "help/color"`. We will add the data of the new page is a simliar format. Here is an example to help.

```yml
# Navigation
...

  Helpful Links:
    - LINK-NAME: "/help/YOUR-PAGE-TITLE/"
```

## Update Git Repository

After adding your help page to the file structure and creating a link in the webpage's basic navigation, we should be update the repository! Doing this depends greatly depends on the environment in which you are working in, but basically we are aiming to push our commited file additions to the repositories origin of the main branch. After doing that the repository will build the new version of the website and you should see your results live!
