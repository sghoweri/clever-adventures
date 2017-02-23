---
title: Typography
---

{% include "@atoms/typography/headings/h1.twig" with {
  heading: {
    text: "Typography"
  }
} %}

Effective typography helps to create an important visual balance on a page—essential for long-format text and marketing copy. By staying consistent with fonts, sizing and spacing, we can create variety in our layouts while still maintaining a sense of context and visual consistency.

{% include "@atoms/typography/headings/h2.twig" with {
  heading: {
    text: "Fonts"
  }
} %}

<a href="https://www.google.com/fonts/specimen/Exo+2">Exo 2</a> is used primarily for headings and titles, including select marketing copy. It was chosen as a natural complement to Open Sans, and is available in a variety of weights, each with a true italic version.

<a href="https://en.m.wikipedia.org/wiki/Open_Sans">Open Sans</a> is the foundation type family for all Pega websites, used for all text with the exception of headlines and titles. With a wide range of weights, and a large diverse character set, the uniform simplicity and legibility over other font families makes Open Sans a great option for presenting information in a variety of languages, which is necessary to bring our content to a global audience.

{% include "@atoms/typography/headings/h2.twig" with {
  heading: {
    text: "Size Standards"
  }
} %}
Our typography sizes are based off of <a href="http://www.modularscale.com/?16&px&1.2&sass&text">1.2 MS Scale</a> with a 16px base. This allows us to create an intuitive visual hierarchy and aesthetically pleasing layout directly in Sass without having to do a bunch of crazy math.

<pre class="language-css u-margin-bottom-large">
  <code>
    $modular-scale: (
      "font_sizes": (
        xxxxlarge:   ms(8),    //  68.797px;
        xxxlarge:   ms(7),    //  57.331px;
        xxlarge:   ms(6),    //  47.776px;
        xlarge:   ms(4),    //  33.178px;
        large:  ms(2),    //  23.04px;
        medium:   ms(1),    //  19.2px;
        base:   ms(0),    //  16.0px;
        small:  ms(-1),   //  14.222px;
        xsmall:  ms(-2)    //  12.642px;
      )
    );
  </code>
</pre>

{% include "@atoms/typography/headings/h2.twig" with {
  heading: {
    text: "Headings"
  }
} %}

Headings (h1 to h6) provide an important way to break up long format text on a web page, and give screen readers and web crawlers, i.e. Google, information about what is important on the page.

Headings should be placed semantically within a layout. Only page titles should be in H1; lower headings should be H2, H3, etc. To achieve a variety of sizes, a set of helper classes is available to content editors so that headings can remain semantic while achieving different visual appearances.


{% include "@atoms/typography/headings/h1.twig" with {
  heading: {
    text: "h1: You have been my friend.",
    classes: "c-heading--xxlarge"
  }
} %}
{% include "@atoms/typography/headings/h2.twig" with {
  heading: {
    text: "h2: That in itself is a tremendous thing.",
    classes: "c-heading--xlarge"
  }
} %}
{% include "@atoms/typography/headings/h3.twig" with {
  heading: {
    text: "h3: I wove my webs for you because I liked you.",
    classes: "c-heading--large"
  }
} %}
{% include "@atoms/typography/headings/h4.twig" with {
  heading: {
    text: "h4: By helping you, perhaps I was trying to lift up my life a trifle.",
    classes: "c-heading--medium"
  }
} %}
{% include "@atoms/typography/headings/h5.twig" with {
  heading: {
    text: "h5: Heaven knows anyone's life can stand a little of that.",
    classes: "c-heading--base"
  }
} %}
{% include "@atoms/typography/headings/h6.twig" with {
  heading: {
    text: "h6: E.B. White, Charlotte's Web",
    classes: "c-heading--base"
  }
} %}