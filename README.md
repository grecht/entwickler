In your `themes` folder use `git submodule add git@github.com:grecht/entwickler.git` to get the theme.

[KaTeX](https://khan.github.io/KaTeX/) support realized with friendly help from [this blog post](http://www.latkin.org/blog/2016/08/07/better-tex-math-typesetting-in-hugo/). Add `hasMath: true` to the front matter of every post containing LaTeX typesetting. Use the following delimiters:

* `\\( MATH \\)` for inline mode
* `$$ MATH $$` for display mode

The menu entries are hardcoded into `header.html`.
