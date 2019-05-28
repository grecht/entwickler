In your `themes` folder use `git submodule add git@github.com:grecht/entwickler.git` to get the theme.

Add `math: true` to the front matter of every post containing LaTeX typesetting. Use the following delimiters:

* `\\( MATH \\)` for inline mode
* `$$ MATH $$` for display mode

Use built-in shortcode [highlight](https://gohugo.io/content-management/syntax-highlighting/) for syntax highlighting.

Example config file:

```
baseurl = "https://wblg.xyz/"
languageCode = "en-us"
title = "Gereon's Weblog"
theme = "entwickler"
ignoreFiles = ["\\.Rmd$", "\\.Rmarkdown$", "_files$", "_cache$"]
preserveTaxonomyNames = true
enableGitInfo = true
footnotereturnlinkcontents = "↩"
pygmentsStyle = "tango"

[permalinks]
    post = "/post/:year/:month/:day/:slug/"
    note = "/note/:year/:month/:day/:slug/"

[params]
    description = "Gereon's Weblog."
    header = ["[Home](/)", "[Photographs](/photographs/)"]
    header_right = ["[About](/about)"]
    footer = ["[Github](https://github.com/grecht)", "[RSS Feed](/index.xml)"]
    email = "gereon@wblg.xyz"
```
