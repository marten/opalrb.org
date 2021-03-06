---
title: "Opal Wrappers"
---

This page is a list of libraries built for opal

## opal-jquery

opal-jquery provides DOM access to opal by wrapping jQuery (or zepto)
and providing a nice ruby syntax for dealing with jQuery instances.
opal-jquery is [hosted on github](http://github.com/opal/opal-jquery).

jQuery instances are toll-free bridged to instances of the ruby class
`JQuery`, so they can be used interchangeably.

```ruby
elements = Element.find('.foo')
# => [<div class="foo">, ...]

elements.class
# => JQuery

elements.on(:click) do
  alert "element was clicked"
end
```
