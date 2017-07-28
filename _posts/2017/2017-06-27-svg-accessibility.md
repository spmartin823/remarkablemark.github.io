---
layout: post
title: Simple SVG accessibility
date: 2017-06-27 23:51:36 -4000
excerpt: A quick way to improve accessibility of SVG files is to update the title and desc elements.
categories: svg accessibility
---

When exporting SVG files with tools like Sketch, you might see something like the following:

```xml
<!-- Generator: Sketch 44.1 (41455) - http://www.bohemiancoding.com/sketch -->
<title>Page 1</title>
<desc>Created with Sketch.</desc>
```

However, the autogenerated [title](https://developer.mozilla.org/docs/Web/SVG/Element/title) and [desc](https://developer.mozilla.org/docs/Web/SVG/Element/desc) are terrible for accessibility because screen readers rely on the metadata for voice over.

As a result, always make it a habit to update these elements:

```xml
<title>Icon</title>
<desc>A description of the icon.</desc>
```