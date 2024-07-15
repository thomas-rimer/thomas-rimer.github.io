---
layout: default
title: Home
---

# Website Outline

Pages
- Pages are written in markdown (this is a page, called index). They contain the content
- At the top of pages are a layout and title
    - The layout references a set of layouts from the /_layouts folder. This layout is default, but there is also grant, page, and post
    - The title is shown in the tab

Sidebar
- The actual structure for the sidebar is contained in the /_includes folder which has sidebar.html
- The inclusion of the sidebar is determined by the whatever the page's layout is, which is saved in the /_layouts folder. Because this page is default, it includes the sidebar. However, other page layouts include footers and other objects from the _includes folder

Misc
- Assets contains images and other local things that 
he default landing page is index.md
- index.md simply contains the 
- Config.yml is design to updated infrequently and contains information about the overall page (edits only visible when you restart the jekyll.serve)

TODO:
- Come up with a favicon and replace existing one
- Replace the LICENSE.md with a proper license
- 
- Figure out what the ogrants.rproj is

BELOW IS CODE FROM THE REUSE.MD page (which I deleted):
## License Summary

Ogrants metadata is available under the [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/) public domain declaration.

Proposal files stored in this repo (proposals/) are made available under the [CC BY 4.0 license](https://creativecommons.org/licenses/by/4.0/), and copyright is retained by the original authors.

The Ogrants website is licensed under the open source [MIT License](https://mit-license.org/).

## Data and Reuse

Metadata is freely available for reuse, per the CC0 license. Use this 
[data download link](export.dat) to obtain a delimited data file.

Reuse of proposal content is governed by their respective license (CC BY 4.0, for proposals downloaded directly from ogrants.org, or the indicated license if a proposal is housed separately).

**Note: Appropriate citation of individual proposals or the metadata is an academic norm, and is recommended for any scholarly outputs that make use of the linked proposal content or metadata.**


{% include footer.html %}
