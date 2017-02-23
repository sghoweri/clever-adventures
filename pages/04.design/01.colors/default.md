---
title: Colors
published: true
visible: true
content:
    items: '@self.children'
    limit: '5'
    order:
        by: date
        dir: desc
    pagination: '1'
    url_taxonomy_filters: '1'
json:
    - colors
---

{% include "@atoms/typography/headings/h1.twig" with {
  heading: {
    text: "Colors"
  }
} %}

Hi!

Our primary and secondary palettes allow us to create a variety of visual components, while keeping a consistent look and feel across websites. The color palettes also help us use and update Sass variables more efficiently, allowing us to change a color once and have it populate everywhere.

Our palettes are always represented as a solid color. For colors that relate to Pega Product families, gradients are used.

{% include "@atoms/typography/headings/h2.twig" with {
  heading: {
    text: "Primary Palette"
  }
} %}

Our primary palette consists of our primary brand color (Pega Blue), and a range of grays that goes from warm (in the lightest shades) to cool (in the darker shades). They should be used for body copy, section backgrounds and links. In body copy, Pega Blue should only be used for links.

For both primary colors, helper classes can be used to lighten or darken the color as needed. .black and .white are separated as their own classes.


{% include "@patterns/01-atoms-01-colors-01-primary-colors@inprogress/01-atoms-01-colors-01-primary-colors@inprogress.markup-only.html" %}

## Secondary colors
Our secondary color palette is used for accent panels, colored tiles and icons. They provide visual variety on the page, but should be used primarily to highlight certain featured items, such as marketing assets or components in Pega Exchange. Secondary colors should never be used for body copy or headlines. Certain colors, such as Teal, may be used for accent text or links. Additionally, they should always be shown as a solid color, and never as part of a gradient.

{% include "@patterns/01-atoms-01-colors-02-secondary-colors@inprogress/01-atoms-01-colors-02-secondary-colors@inprogress.markup-only.html" %}

{% include "@atoms/typography/headings/h2.twig" with {
  heading: {
    text: "Product gradients"
  }
} %}

Product gradients are used primarily to represent products in the Pega family, and are named according to each product. They should be used only in connection to content or page components that relate to a specific product.

{% include "@patterns/01-atoms-01-colors-03-gradients@inprogress/01-atoms-01-colors-03-gradients@inprogress.markup-only.html" %}
