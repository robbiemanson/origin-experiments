---
categories: utilities
layout: page
scss-filename: _flex-direction.scss
title: flex-direction
---
Mixin and utility classes to apply `flex-direction` values.

The `flex-direction` property specifies how flex items are placed in the flex container, by setting the direction of the flex container's main axis. This determines the direction that flex items are laid out in.

[http://w3.org/tr/css3-flexbox/#flex-direction-property](http://w3.org/tr/css3-flexbox/#flex-direction-property)

This work is derived from [sass-flex-mixin](https://github.com/mastastealth/sass-flex-mixin).

### Values
* `column`
* `column-reverse`
* `row` (default)
* `row-reverse`

### Examples
<div class="DocsExample DocsExample--grouped DocsExample--labelUtilityClasses">
{% example html %}
<div class="flexbox flex-direction--column">
  <div class="background-color--gray-15">Flex item one</div>
  <div class="background-color--gray-13">Flex item two</div>
  <div class="background-color--gray-12">Flex item three</div>
</div>
{% endexample %}
</div>

<div class="DocsExample DocsExample--labelMixins DocsExample--renderHidden">
{% example scss %}
.MyComponent {
  @include flexbox;
  @include flex-direction(column);
}
{% endexample %}
</div>


<div class="DocsExample DocsExample--grouped DocsExample--labelUtilityClasses">
{% example html %}
<div class="flexbox flex-direction--column-reverse">
  <div class="background-color--gray-15">Flex item one</div>
  <div class="background-color--gray-13">Flex item two</div>
  <div class="background-color--gray-12">Flex item three</div>
</div>
{% endexample %}
</div>

<div class="DocsExample DocsExample--labelMixins DocsExample--renderHidden">
{% example scss %}
.MyComponent {
  @include flexbox;
  @include flex-direction(column-reverse);
}
{% endexample %}
</div>


<div class="DocsExample DocsExample--grouped DocsExample--labelUtilityClasses">
{% example html %}
<div class="flexbox flex-direction--row">
  <div class="background-color--gray-15">Flex item one</div>
  <div class="background-color--gray-13">Flex item two</div>
  <div class="background-color--gray-12">Flex item three</div>
</div>
{% endexample %}
</div>

<div class="DocsExample DocsExample--labelMixins DocsExample--renderHidden">
{% example scss %}
.MyComponent {
  @include flexbox;
  @include flex-direction(row);
}
{% endexample %}
</div>


<div class="DocsExample DocsExample--grouped DocsExample--labelUtilityClasses">
{% example html %}
<div class="flexbox flex-direction--row-reverse">
  <div class="background-color--gray-15">Flex item one</div>
  <div class="background-color--gray-13">Flex item two</div>
  <div class="background-color--gray-12">Flex item three</div>
</div>
{% endexample %}
</div>

<div class="DocsExample DocsExample--labelMixins DocsExample--renderHidden">
{% example scss %}
.MyComponent {
  @include flexbox;
  @include flex-direction(row-reverse);
}
{% endexample %}
</div>
