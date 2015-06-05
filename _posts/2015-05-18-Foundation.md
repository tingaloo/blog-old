---
layout: post
title: 'Foundation'
quote: "Grids Check. Responsive Check."
date: 2015-05-18
categories: [Web Development]
---

## Responsive.

I try to use Foundation as much as possible. This grid system is very familiar and as a whole responsive.

## Overrides.
Only problems is overriding attributes that are default in the framework.
For example, the last child of an index would be floated right. But I would not know that until I found the conflict through the developer console.

  It overrided many button styles I was always building inside the grid wrapper. Sometimes there would be no conflicts, sometimes I had to fight the framework to get my button styles in. Thankfully there is a community out there that already experienced the conflicts I had.

## With Rails
I re-ordered my overrides in application.css.scss

```scss

 *= require "framework_and_overrides"
 *= require "book_checkouts"
 *= require "books"
 *= require "users"
 *= require_self
 */
```
This makes it so that foundation's overrides get handled first, then my custom styles will not be overriden.

## Finally
Foundation is neat to have around. It is a bloated framework, but it is neatly documented and easy to comment out features I don't need.








