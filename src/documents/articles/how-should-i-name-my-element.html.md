---
title: How should I name my element?
author: zeno_rocha
date: 2014-03-12
image: how-should-i-name-my-element.jpg
category: articles
layout: single
tags: ['Best Practices', 'Custom Elements']
---

Naming is always a challenging task when developing a component. We can create
truly complex pieces of code but we still have a hard time to name a simple
variable. The same is true for naming custom elements and we're here today to
help with you that.

<!-- Read more -->

## &lt;oneword&gt; vs &lt;two-words&gt;

Although using just one word for your element seems pretty handy (e.g
`<tabs>`), according to the [spec](http://www.w3.org/TR/custom-elements/)
your element need to have a dash in its name (e.g `<johns-tabs>`). That
way you're forced to add a namespace which avoids conflits with existing
elements.

Some people use the x-* prefix when they have a single word element that doesn't
make sense to break apart like `<x-instagram>` instead of `<insta-gram>`.

## &lt;polymer-something&gt; & &lt;x-something&gt;

Nowadays we've been using libraries like [Polymer](http://www.polymer-project.org/)
and [X-Tag](http://x-tags.org/) to help us write custom elements.
Those libraries usually include a prefix to identify their elements (e.g
`<polymer-something>`, `<x-something>`), so when people create an element using
Polymer for example they also include this polymer-* prefix.

This is considered a bad practice, because we don't want to build a world where
elements are seen as being "owned" by Polymer or X-Tag or whatever framework may
later come along.

The text before the dash is effectively a namespace and you should want to keep
it short but also unique. Try not to overlap on someone else's prefix if
possible.

## What about you?

Tell us below how do you usually name your elements and share your thoughts
about your own custom elements naming conventions.
