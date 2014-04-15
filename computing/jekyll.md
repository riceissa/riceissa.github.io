---
layout: default
title: Setting up Jekyll on GitHub
---

I think Jekyll is designed to run automatically on GitHub, as long as you are in your website repository (<code>USERNAME.github.io</code>) or in the <code>gh-pages</code> branch in any other repository.

The most important file is called <code>\_config.yml</code>, and must be placed in the main directory.
If one is using GitHub pages on one’s website repository, it should look like:

    markdown: redcarpet
    baseurl: ""
    exclude: ['README.md']

For any other repository, the <code>baseurl</code> must be modified:

    markdown: redcarpet
    baseurl: /REPONAME
    exclude: ['README.md']

## References

- See [Thomas Bradley’s guide](https://github.com/algonquindesign/jekyll) (there are also video tutorials, which can be accessed from that page).

- See also [my own Quora post about static page generation](https://www.quora.com/Issa-Rice/Data-Archiving/Static-page-generation).
