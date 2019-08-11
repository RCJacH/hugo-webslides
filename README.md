![Screenshot](https://raw.githubusercontent.com/rcjach/hugo-webslides/master/images/screenshot.png)

# Hugo-WebSlides

Hugo-WebSlides is a theme for writing beautiful [WebSlides](https://webslides.tv) presentations in markdown with [Hugo](https://gohugo.io/).

Features:
- Based on WebSlides.js
- Create slides with Markdown.
- Assign classes to elements without html.
- Shortcodes for components.

Future Implementation:
- More component shortcodes!
- Hugo-WebSlides rendition of [original demos](https://webslides.tv/demos/).
- Separate slides within the same project.

## Demo

[Checkout the latest **demo**](https://rcjach.github.io/hugo-webslides) of what you can create with this theme.


# Getting Started
## Requirements

Installation of [Hugo](https://gohugo.io/) (latest version recommended)

## Get the theme

Run from the root of your Hugo site:
```sh
$ git clone https://github.com/rcjach/hugo-webslides.git themes/hugo-webslides
```

Alternatively, you can include this repository as a [git submodule](https://git-scm.com/book/de/v1/Git-Tools-Submodule). This makes it easier to update this theme if you have your Hugo site in git as well:

```sh
$ git submodule add https://github.com/rcjach/hugo-webslides.git themes/hugo-webslides
```

## Preview the theme

Hugo-WebSlides ships with an fully configured example site. For a quick preview:

```
cd exampleSite/
hugo serve  --themesDir ../..
```

Then visit `http://localhost:1313/` in your browser to view the example site.

## Configuration


The following `config.toml` is used for the example site.

```toml
baseurl         = "/"
theme           = "hugo-webslides"
languageCode    = "en-us"
title           = "A Hugo theme for creating Webslides.js presentations"

[params]
  author = "RCJacH"
  homepage = "RCJacH.github.io"

[params.webslides]
  banner = false
  slideshow = true
  vertical = false
  autoslide = false
  changeOnClick = false
  disableLoop = false
  minWheelDelta = 40
  disableNavigateOnScroll = false
  scrollWait = 450
  slideOffset = 50
  hideIndex = false

[blackfriday]
extensionsmask = ["autoHeaderIds"]
```

Checkout [WebSlides Core-API options](https://github.com/webslides/WebSlides/wiki/Core-API#options) for an explanation of what different parameters do.

Note that some parameters is inverted in this theme, for example loop -> disableLoop, navigateOnScroll -> disableNavigateOnScroll, showIndex -> hideIndex.

## Adding content

For minimum work, simply copy the content folder of the exampleSite to your project, and modify the existing md files to your need.


Split slides by using horizontal ruler `---`.
```md
Slide 1

---

Slider 2
```

## Assign properties

Use HTML comment with a colon to add properties to a slide or an element.
<!-- : assignment -->

### Slide properties

You can assign the following properties to each slide:
- section class
- div class
- secondary div class
- background class
- background-image
- background-image-position

~~~md
<!-- : sectionClass .divClass ..secondaryClass bg=backgroundClass bgimage=background-image bgpos=background-image-position -->
~~~

Multiple classes can be assigned.

~~~md
<!-- : .divClass1 .divClass2 ..secondaryDivClass1 ..secondaryDivClass2 bg=backgroundClass1 bg=backgroundClass2 -->
~~~

### Block properties

You can assign classes to blocks as well.

```md
### <!-- : .headerClass -->Header
<!-- : .paragraphClass -->Paragraph
```
