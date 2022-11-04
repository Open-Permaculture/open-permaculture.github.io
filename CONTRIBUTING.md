---
layout: default
title: Contributing
nav_exclude: true
search_exclude: true
---

# Contributing:

## Set up:

openpermaculture.com is hosted on GitHub pages. In order to contribute to openpermaculture.com you will need a GitHub account. 

Once you have created a GitHub account navigate to the openpermaculture repository [here](https://github.com/Open-Permaculture/open-permaculture.github.io).

There you will see the folder structure that contains the code for the website. Pages are .md files that allow you to write in a format similar to BB code found on most online forums.

You can download the entire website by clicking the green code button and then "Download ZIP" from there you can edit any pages you want. When you decide you are ready to post your changes you need to click the contribute button and upload the files you have modified. A moderator will then review your changes and merge them with the main repository.

You may also create a fork of the project which will create a copy of the repository in your account's repositories which you may sync with the original or edit and request a merge.

## Editing a page:

If you just want to modify a single page then navigate to the page in the GitHub repo and click the pencil button, make your changes then open a pull request.

### Adding text:

There are three options for formatting text on a page, they can all be used at the same time.

* GitHub's [markdown](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax) (similar to BB code)
* Raw [html](https://html.com/) code.
* Jekyll [theme markdown](https://github.com/Open-Permaculture/just-the-docs/blob/main/docs/index-test.md). 

## Guidelines:

When adding/changing text we want to ensure the voice (how pages read) remains consistent across all pages.

### Maintain a neutral worldview:

* DO NOT: Use personification when referring to earth/nature, for example, Gaia, mother earth, etc.
* DO NOT: Refer to earth/nature with a worldview bias, for example, creation, cosmic mistake, etc.
* DO NOT: Make theoretical statements outside of recorded history, for example: "millions of years ago X happened" or "as a result of X prehistoric catastrophic event...".
* DO NOT: Make claims about the shape of the earth such as round, flat, or hollow. These are generally outside of what the reader can test for themselves.
* DO NOT: Make political or opinion statements, for example: "if we don't act now civilization will burn" or "vote for X politician".

### Other launage guidelines:

* DO NOT: Contribute information that is not repeatable, observable science that the reader can test for themselves.
* DO NOT: Use profane or inappropriate language. No butts no nuts no coconuts.
* DO NOT: Plagerize any images or text from other works without proper references. Citations should be made in MLA format.

Keep in mind any information contributed will be released into public domain under the CC-BY-SA (Creative Commons By Attribution Sharealike license).

The purpose of these guidelines is to make sure that the information is practical & actionable information without alienating any particular group. However, the "Why permaculture?" page will try to cover many of the different reasons why people may want to use it. 

If you would like to create information that is outside these guidelines for a specific people group or belief system you may create a fork of the project, however, the information approved for openpermaculture.com must remain a neutral baseline.

### Adding an image:

First, add your image to the assets/images folder. Ideally, the image should be a .jpg file and no more than 800px wide, .png & .gif are also supported.

Add the image using:
```
![](/assets/images/open-permaculture-github-banner.jpg)
```

### Adding a YouTube video:

```
<iframe width="420" height="315"
src="https://www.youtube.com/embed/your-video-id">
</iframe>
```

Please be sure that embedded videos that include text and/or audio also conform to the guidelines.

### Adding a graph:

Jekyll theme markdown enables mermaid for graph rendering, see this [link](https://mermaid-js.github.io/mermaid/#/README) for how to use it.

## Adding a new chapter/section:

The navigation structure is formatted by the website's Jekyll theme which you can learn about [here](https://just-the-docs.github.io/just-the-docs/docs/navigation-structure/).

To add a new chapter create a new folder ```chapter-name``` add create a new file ```chapter-name.md``` inside that folder with the following header at the top of the file:
```
---
layout: default
title: Chapter Name
nav_order: 1
parent: Chapters
---
```

nav_order determines chapter order if left at 1 then the chapter will be the first chapter.

To add a section to the chapter add a new file named ```section-name.md``` inside the folder of the chapter it is a part of. The header for a section is:
```
---
layout: default
title: Section Name
nav_order: 1
parent: Chapter Name
grand_parent: Chapters
---
```

nav_order determines section order if left at 1 then the section will be the first section.