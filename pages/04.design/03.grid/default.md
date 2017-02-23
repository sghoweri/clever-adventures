---
title: Grid
---

{% include "@atoms/typography/headings/h1.twig" with {
  heading: {
    classes: "c-heading--xxlarge",
    text: "Grid"
  }
} %}

Our grid system is based off of Harry Robert's framework-less <a href="http://csswizardry.com/csswizardry-grids/
https://github.com/csswizardry/discovr/blob/master/css/trumps/_trumps.widths.scss">CSS grid system.</a> The grid separates the layout from content and is baked into the components. All Pega sites use a responsive, Sass-based grid inspired by [CSS Wizardry Grid](https://github.com/csswizardry/csswizardry-grids).The grid is flexible enough to create a variety of layouts, from a single-column layout to complex layouts created by breaking the page into up to six columns, and combining columns from there.

<div class="o-grid u-margin-bottom-large o-grid--flex">
  
  <div class="o-grid__item u-1/1">
    {% include "@molecules/grid/grid-demo.twig"%}
  </div>

  <div class="o-grid__item u-1/2">
    {% include "@molecules/grid/grid-demo.twig" with {
      grid_text: "1/2"
    } %}
  </div>
  
  <div class="o-grid__item u-1/2">
    {% include "@molecules/grid/grid-demo.twig" with {
      grid_text: "1/2"
    } %}
  </div>
  
  <div class="o-grid__item u-1/3">
    {% include "@molecules/grid/grid-demo.twig" with {
      grid_text: "1/3"
    } %}
  </div>
  
  <div class="o-grid__item u-1/3">
    {% include "@molecules/grid/grid-demo.twig" with {
      grid_text: "1/3"
    } %}
  </div>
  
  <div class="o-grid__item u-1/3">
    {% include "@molecules/grid/grid-demo.twig" with {
      grid_text: "1/3"
    } %}
  </div>

    <div class="o-grid__item u-1/4">
    {% include "@molecules/grid/grid-demo.twig" with {
      grid_text: "1/4"
    } %}
  </div>
  
  <div class="o-grid__item u-1/4">
    {% include "@molecules/grid/grid-demo.twig" with {
      grid_text: "1/4"
    } %}
  </div>
  
  <div class="o-grid__item u-1/4">
    {% include "@molecules/grid/grid-demo.twig" with {
      grid_text: "1/4"
    } %}
  </div>
  
  <div class="o-grid__item u-1/4">
    {% include "@molecules/grid/grid-demo.twig" with {
      grid_text: "1/4"
    } %}
  </div>

  <div class="o-grid__item u-1/5">
    {% include "@molecules/grid/grid-demo.twig" with {
      grid_text: "1/5"
    } %}
  </div>
  
  <div class="o-grid__item u-1/5">
    {% include "@molecules/grid/grid-demo.twig" with {
      grid_text: "1/5"
    } %}
  </div>
  
  <div class="o-grid__item u-1/5">
    {% include "@molecules/grid/grid-demo.twig" with {
      grid_text: "1/5"
    } %}
  </div>
  
  <div class="o-grid__item u-1/5">
    {% include "@molecules/grid/grid-demo.twig" with {
      grid_text: "1/5"
    } %}
  </div>
  
  <div class="o-grid__item u-1/5">
    {% include "@molecules/grid/grid-demo.twig" with {
      grid_text: "1/5"
    } %}
  </div>

  <div class="o-grid__item u-1/6">
    {% include "@molecules/grid/grid-demo.twig" with {
      grid_text: "1/6"
    } %}
  </div>
  
  <div class="o-grid__item u-1/6">
    {% include "@molecules/grid/grid-demo.twig" with {
      grid_text: "1/6"
    } %}
  </div>
  
  <div class="o-grid__item u-1/6">
    {% include "@molecules/grid/grid-demo.twig" with {
      grid_text: "1/6"
    } %}
  </div>
  
  <div class="o-grid__item u-1/6">
    {% include "@molecules/grid/grid-demo.twig" with {
      grid_text: "1/6"
    } %}
  </div>
  
  <div class="o-grid__item u-1/6">
    {% include "@molecules/grid/grid-demo.twig" with {
      grid_text: "1/6"
    } %}
  </div>
  
  <div class="o-grid__item u-1/6">
    {% include "@molecules/grid/grid-demo.twig" with {
      grid_text: "1/6"
    } %}
  </div>
</div>



Unlike bootstrap, this grid is built as you go. There are no pre-defined columns or rows. To start, in a .twig file use the code below to define the grid:

```HTML
<div class="o-grid">
	<div class="o-grid__item"></div>
</div>
```

Rows and columns can now be thought of as cells which are defined by fractions For example, to create a two column layout add:
```HTML
<div class="o-grid">     
  <div class="o-grid__item u-1/2"></div>
      
  <div class="o-grid__item u-1/2"></div>
</div>
```

This creates two equal columns:
<div class="o-grid">
  
  <div class="o-grid__item u-1/2">
  {% include "@molecules/grid/grid-demo.twig" with {
    grid_text: "1/2"
  } %}
  </div>
  <div class="o-grid__item u-1/2">
  {% include "@molecules/grid/grid-demo.twig" with {
    grid_text: "1/2"
  } %}
  </div>
</div>

A traditional two-column layout with a left sidebar and wide content area can be created by breaking the layout into 5 columns, and creating one cell of 2/5 and another of 3/5:

```HTML
<div class="o-grid">
	<div class="o-grid__item u-2/5"></div>

	<div class="o-grid__item u-3/5"></div>
</div>
```

<div class="o-grid">
  <div class="o-grid__item u-2/5">
  {% include "@molecules/grid/grid-demo.twig" with {
    grid_text: "2/5"
  } %}
  </div>
  <div class="o-grid__item u-3/5">
  {% include "@molecules/grid/grid-demo.twig" with {
    grid_text: "3/5"
  } %}
  </div>
</div>

Our grid system employs a mobile first approach. Thus, breakpoints start at small screens and expand to larger screen widths. This means that a single-column grid will remain single-column whether it’s on a user’s mobile device or on their laptop. To display cells at full width only at the small breakpoint (typical for responsive sites), you can use @[breakpoint] to customize the grid:

```HTML
<div class="o-grid"> 
      <div class="o-grid__item u-1/1 u-1/2@small">
      </div>
      
      <div class="o-grid__item u-1/1 u-1/2@small">
      </div>
    </div>
```
    
This creates a two-column grid that collapses to a single stacked column on smaller breakpoints.

<div class="o-grid">  
  <div class="o-grid__item u-1/1 u-1/2@small">
  {% include "@molecules/grid/grid-demo.twig" with {
    grid_text: "u-1/1 u-1/2@small"
  } %}
  </div>
  <div class="o-grid__item u-1/1 u-1/2@small">
  {% include "@molecules/grid/grid-demo.twig" with {
    grid_text: "u-1/1 u-1/2@small"
  } %}
  </div>
</div>