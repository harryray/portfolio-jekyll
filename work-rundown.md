---
layout: page_two-col
no-padding: true
full-width: true
title: Work Rundown
permalink: /work-rundown/
thumbnail: https://picsum.photos/800/300/?image=47
main_image: https://picsum.photos/1200/1920/?image=47
---

{{ site.description }}

This is based on the `Minima` Jekyll theme. I've customised it fairly heavily, particularly the homepage. This involved a couple of hours of tweaking, but is largely styling changes, making use of BEM and SASS to ensure a concise, easy-to-maintain stylesheet, compiled with Jekyll into CSS.

I've also built a custom layout (`page_two-col`), which is what this page is using. The image is set in a variable in the front matter for this page, along with the thumbnail. I'm using picsum.photos to get images for this site as I've found they're the best placeholders; plenty of variety, and always high-res.

This is the first site that I've built with Jekyll (started around 05/02/2019), so I'm basically just playing around with fairly simple things at the moment, adding variables to the front matter for use in styling, adding custom layouts, etc.

I've been experimenting with some non-standard layouts, which you'll see on the homepage; wrapper-breaking elements (the instagram section), vertical block titling, and big text.

The instafeed integration was a little trickier than it would usually be, because Jekyll runs on Liquid. When using the `template` parameter for instafeed, liquid tries to render the tags that instafeed makes use of, due to the syntax they use. The workaround is to assign the strings used for instafeed (e.g `{% raw %}{{image}}{% endraw %}`) to a variable for liquid (e.g `{% raw %}{% assign insta_image = '{{image}}' %}{% endraw %}`), and use that in place.

You can view my main site [here](https://harry-ray.com) or my tech portfolio [here](https://harryray.github.io/harry-ray/).

You can find the source code for Minima at GitHub:
[jekyll][jekyll-organization] /
[minima](https://github.com/jekyll/minima)

You can find the source code for Jekyll at GitHub:
[jekyll][jekyll-organization] /
[jekyll](https://github.com/jekyll/jekyll)


[jekyll-organization]: https://github.com/jekyll
