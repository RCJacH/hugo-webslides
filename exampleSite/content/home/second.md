+++
title = "Hugo-Webslides"
weight = 1
+++
<!--: .wrap .size-70 ..aligncenter -->


## <!--  --> **Hugo-Webslides**
<!--: .text-intro -->Use markdown to write contents and render with **WebSlides** to html.

[{{< svg fa-github >}}Github](https://github.com/RCJacH/hugo-webslides)

---
<!-- : .wrap -->

### **Get the theme**
<!-- : .text-intro -->Run from the root of your Hugo site:
~~~
$ git clone https://github.com/RCJacH/hugo-webslides.git themes/hugo-webslides
~~~

---

<!--: .wrap -->

## **WebSlides Demos**
Here's what you can do with [WebSlides](https://webslides.tv).

<!--: .flexblock gallery -->
- {{< gallery title="Why WebSlides" href="https://webslides.tv/demos/why-webslides" src="https://webslides.tv/static/images/demos-why.png" >}}Why WebSlides{{< /gallery >}}
- {{< gallery title="Landings" href="https://webslides.tv/demos/landings" src="https://webslides.tv/static/images/demos-landings.png" >}}Landings{{< /gallery >}}
- {{< gallery title="Portfolios" href="https://webslides.tv/demos/portfolios" src="https://webslides.tv/static/images/demos-portfolios.png" >}}Portfolios{{< /gallery >}}
- {{< gallery title="Keynote" href="https://webslides.tv/demos/apple" src="https://webslides.tv/static/images/demos-apple.png" >}}Keynote{{< /gallery >}}

---
<!--: .wrap -->

## **More Examples**
<small>Note. None of these slides are currently not ported to Hugo-Webslides...YET.</small>

<!--: .flexblock gallery -->
- {{< gallery title="Netflix's Culture" href="https://webslides.tv/demos/netflix-culture" src="https://webslides.tv/static/images/demos-netflix.png" >}}Netflix{{< /gallery >}}
- {{< gallery title="Longform Articles" href="https://webslides.tv/demos/longforms" src="https://webslides.tv/static/images/demos-longforms.png" >}}Longforms{{< /gallery >}}
- {{< gallery title="Interviews" href="https://webslides.tv/demos/interviews" src="https://webslides.tv/static/images/demos-interviews.png" >}}Interviews{{< /gallery >}}

---
<!-- : .wrap -->

|||v

### **Settings**
<!-- : .text-intro -->You can modify WebSlides configuration directly from config.toml.


|||

~~~toml
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
~~~




