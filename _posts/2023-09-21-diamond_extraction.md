---
layout: post
title: Extract diamond from image
date: 2023-09-20 08:57:00-0400
description: Extract the diamond from the given images.
tags: images background-removal convex-hull
categories: image-processing
giscus_comments: true
related_posts: false
featured: true
---

{::nomarkdown}
{% assign jupyter_path = "assets/jupyter/extract_diamond.ipynb" | relative_url %}
{% capture notebook_exists %}{% file_exists assets/jupyter/extract_diamond.ipynb %}{% endcapture %}
{% if notebook_exists == "true" %}
    {% jupyter_notebook jupyter_path %}
{% else %}
    <p>Sorry, the notebook you are looking for does not exist.</p>
{% endif %}
{:/nomarkdown}
