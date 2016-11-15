jekyll-reveal-template
======================


? do you have to specify text/template for all sections, or can you wrap the whole thing in that and do markdown?




Boilerplate to start a [reveal.js](https://github.com/hakimel/reveal.js/) slideshow with Jekyll on GitHub Pages.

You can check the current versions of github-pages [dependencies](https://pages.github.com/versions/) by `github-pages versions` (though former lists ruby version).

GitHub pages reveals GitHub [metadata](https://help.github.com/articles/repository-metadata-on-github-pages/).

## Using

1. clone repo
2. create Jekyll page with `layout: slide`

## Layout

Two layouts are provided:

1. `slide`
2. `slide-md`

The `slide` layout is appropriate for 

Note that Jekyll will attempt to process markdown files

? Is it possible to have jekyll process the markdown then hand it off to reveal in sections?


## Configuration and Customization

Options should given in YAML front matter like:

    reveal:
      theme: night
      transition: slide
      width: 1680
      height: 1050

### Available Options

See [Configuration](https://github.com/hakimel/reveal.js#configuration), [Presentation Size](https://github.com/hakimel/reveal.js#presentation-size), and [Theming](https://github.com/hakimel/reveal.js#theming)

option     | default   | values
-----------|-----------|-------
theme      | black     | see [Theming](https://github.com/hakimel/reveal.js/#theming)
transition | 'slide' | none/fade/slide/convex/concave/zoom
width      | 960       | px or %
height     | 700       | px or %
controls   | true      | true/false
progress   | true      | true/false
history    | false     | true/false
center     | true      | true/false

## Layout details

- Reveal.js Jekyll layout based on [slide.html](https://gist.github.com/luugiathuy/c07ac5608addadb642e5#file-slide-html) (see [blog post](http://luugiathuy.com/2015/04/jekyll-create-slides-with-revealjs/))
- Updated dependencies as per reveal [README](https://github.com/hakimel/reveal.js#dependencies)
- Change the way `theme` and `transition` are set in YAML (e.g. from `theme` to `reveal.theme`), and add additional configuation options
- Add ability to specify additional options in page YAML, including width and height.


