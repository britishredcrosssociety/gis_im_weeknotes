# About
A minisite to share weeknotes from the BRC GIS and IM Team
https://britishredcrosssociety.github.io/gis_im_weeknotes/

The site is built using [11ty](https://www.11ty.dev/), which converts Markdown to HTML using Javascript. It's hosted on GitHub pages. 

## Setup instructions
1. Install [node.js](https://nodejs.org/en) (version 18 or above). For BRC laptops, this is available on Company Portal.
2. Clone the directory: `git clone https://github.com/britishredcrosssociety/gis_im_weeknotes.git`
3. Run `npm install` to install the JavaScript dependencies
4. Run `npx @11ty/eleventy` to generate the HTML content. By default this will be saved in the `doc` folder

## Making new weeknotes
1. Make a new Markdown file in `content/blog` named with the date. (By convention, we're using the last working day of the week that the weeknote refers to)
2. Fill in the frontmatter for the markdown file:
```
---
title: The title for the post
date: yyyy-mm-dd
draft: true/false
---
```
3. Write the content beneath in Markdown
4. Rebuild the HTML with `npx @11ty/eleventy` (run from the base directory)
   * To preview changes locally, run `npx @11ty/eleventy --serve`
6. Add changed files with `git add *`
7. Commit with `git commit -m "Add: weeknotes for week yyyy-mm-dd"`
8. Push changes to Github `git push`
(Or commit changes and push using GitHub desktop)
