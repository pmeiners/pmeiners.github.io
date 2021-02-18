---
layout: post
title:  "First Post"
date:   2021-02-17 23:58:21 +0100
categories: jekyll update
---

So I've finally created my own website, and you've decided to read this post. 

## Jekyll
This website is built with jekyll, and it is (obviously) hosted on github pages. Why jekyll?

The installation of jekyll is not that straightforward, unfortunately. The documentation for installing jekyll on MacOS is in some places outdated, which means that you'll have to scour the web and find your own method. Creating a site with RMarkdown through Hugo might be more straightforward.

However, the base jekyll website you see here is surprisingly simple to edit. Instead of going through several layers of RStudio, YAML, etc., you can just edit posts in good old non-fancy markdown.

It is also much more lightweight than hosting your own WordPress instance and having to deal with theme updates that break your site. 
In comparison to WordPress, you can export to other services if Github Pages disappears in the future.

## Content

I do not plan to update the blog part of this site too frequently. I have some ideas for toy empirical examples. Overall, the content will probably be similar to a long twitter thread.

Luckily, you can also include code snippets in your post:

{% highlight r %}
library (tidyverse)
data_all <- coast_vs_waste %>% 
  left_join(mismanaged_vs_gdp, by = c("Code", "Year")) %>%
  left_join(waste_vs_gdp, by = c("Code", "Year"))
{% endhighlight %}

So expect some R code.


