---
layout: post
title: "The @noescape tag purpose and why it must be explicitly applied"
date: 2016-01-13 21:49:49 +0100
comments: true
categories: closures
author: David Cordero
---


This week [I](https://github.com/dcordero) had a very interesting discussion about `@autoclosures` and `@noescape` tags with [@phelgo](https://github.com/phelgo), as result of which we wondered the whys of some decision in the design of Swift's syntax.

More specifically we are wondering why the tag `noescape` isn't automatically detected and it needs to be explicitly applied. Because... In fact, it is somehow detected at compile time, because trying to add the @noescape tag to a func with escaping closures results in an error.

So the question is why... why noescape needs to be explicitly added and Apple did not create it to be automatically added when it is needed?

[...]
