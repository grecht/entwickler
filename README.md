In your `themes` folder use `git submodule add git@github.com:grecht/entwickler.git` to get the theme.

[KaTeX](https://khan.github.io/KaTeX/) support realized with friendly help from [this blog post](http://www.latkin.org/blog/2016/08/07/better-tex-math-typesetting-in-hugo/). Add `hasMath: true` to the front matter of every post containing LaTeX typesetting. Use the following delimiters:

* `\\( MATH \\)` for inline mode
* `$$ MATH $$` for display mode

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
    header =  ["[Home](/)", "[Photographs](/photographs/)"]
    header_right = ["[About](/about)"]
    footer = "&#169; Gereon Recht | [Home](/) [Github](https://github.com/grecht) | "
    email = "gereon@wblg.xyz"

```
