---
categories: utilities
layout: page
scss-filename: _float.scss
title: float
---
Use to apply `float` values with utility classes, and ‘clearfix’ hack with a mixin or utility classes. Values can optionally be applied only at specific [breakpoints]({{ site.baseurl }}/utilities/breakpoint).

Related: [clear]({{ site.baseurl }}/utilities/clear)

### Values
* `left`
* `none`
* `right`

### Examples
<div class="DocsExample DocsExample--grouped DocsExample--labelUtilityClasses">
{% example html %}
<div class="floatContainer">
  <div class="background-color--gray-13 float--left">
    This element floats to the left
  </div>
</div>
{% endexample %}
</div>

<div class="DocsExample DocsExample--labelCSS DocsExample--renderHidden">
{% example scss %}
.MyComponent {
  @include floatContainer;
}

.MyComponent-child {
  float: left;
}
{% endexample %}
</div>


<div class="DocsExample DocsExample--grouped DocsExample--labelUtilityClasses">
{% example html %}
<div class="floatContainer">
  <div class="background-color--gray-13 md-float--right">
    This doesn't float until the medium breakpoint, when it floats to the right
  </div>
</div>
{% endexample %}
</div>

<div class="DocsExample DocsExample--labelCSS DocsExample--renderHidden">
{% example scss %}
.MyComponent {
  @include floatContainer;
}

.MyComponent-child {
  @include break(md) {
    float: right;
  }
}
{% endexample %}
</div>


<div class="DocsExample DocsExample--grouped DocsExample--labelUtilityClasses">
{% example html %}
<div class="floatContainer">
  <div class="background-color--gray-13 float--none">
    This element would have any inherited float removed
  </div>
</div>
{% endexample %}
</div>

<div class="DocsExample DocsExample--labelCSS DocsExample--renderHidden">
{% example scss %}
.MyComponent {
  @include floatContainer;
}

.MyComponent-child {
  float: none;
}
{% endexample %}
</div>
