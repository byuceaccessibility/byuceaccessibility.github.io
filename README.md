# BYU CE Accessibility

[![Open in Visual Studio Code](https://img.shields.io/badge/Open%20in-Visal%20Studio%20Code-blue?style=for-the-badge&logo=visualstudiocode)](https://open.vscode.dev/byuceaccessibility/byuceaccessibility.github.io)

Accessibility Help page for BYU CE employees.

# Getting Started

# Adding a Help Page

Adding a help page is very simple. It only requires knowlegdge on the use of a markdown file. If you don't know what 'markdown' is, markdown is a simplified html file. For examples and a how to write in 'markdown' see [Docs Markdown reference](https://docs.microsoft.com/en-us/contribute/markdown-reference) from Microsoft.

## A File to folder structure

To start make a new file in the `help\` folder of this respository. Title it using the markdown file exenstion (`YOUR-TITLE.md`). In that file is where we will put all of the content of your new help page.

Copy the text in the next paragraph to your new files contents. This will be the basis we will start the page with.

```markdown
---
layout: page
title: YOUR-PAGE-TITLE
permalink: /help/YOUR-PAGE-TITLE
---

Your page content...
```

In the prior example code you will see data between lines of hyphens, `---`, and `Your page content...`. The data between the lines of hypens are values that will fill in the basic webpage layout out and make your page match the rest of the website. `Your page content...` is simply filler text that you can replace with markdown of your choice.

## A File to webpage navigation

Now that you've added the file to our repository, we need to add your page to the basic navigation of the website so people can access it. To do this we will add the title and path to the `_config.yml` file in the base folder of this directory.

Open `_config.yml` and find the 