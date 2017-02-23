---
title: 'Atomic Design'
---

{% include "@atoms/typography/headings/h1.twig" with {
  heading: {
    classes: "c-heading--xxlarge",
    text: "Atomic Design"
  }
} %}

The web moves fast. Where once we could get away with designing pages as discrete objects, modern web design requires a design system that builds from the ground up, allowing us to iterate quickly while maintaining a consistent look and feel across
properties. By creating a rich, versatile library of reusable components, we can add new layouts quickly, without building up new [technical or design debt](http://en.wikipedia.org/wiki/Technical_debt). While a new campaign or feature might require
the creation of a new component, new patterns come at a high cost—they require new design elements, additional code, maintenance, and they increase the [cognitive load](http://en.wikipedia.org/wiki/Cognitive_load) on users. The public part of this
guide focuses on the atoms - the basic building blocks of our digital presence. For an ongoing reference to the rest of our design patterns, visit our [Pattern Lab](http://vpatternlab/) instance (only available on Pega's network).

{% include "@atoms/typography/headings/h2.twig" with {
  heading: {
    text: "Atomic what, now?"
  }
} %}

Atomic design flips the traditional model of web layout on its head. Rather than designing discrete *page templates* and breaking them down into CSS components, atomic design starts from the base-level components and works up to finished designs:

<div class="o-grid o-grid--flex">
<div class="o-grid__item u-1/1 u-1/2@small u-margin-bottom">
{% embed "@molecules/tiles/tile.twig" with {
  tile: {
    classes: "c-tile--small u-background-color-light-gray"
  }
} %}
  {% block tile_content %}
    {% include "@atoms/typography/headings/h3.twig" with {
      heading: {
        text: "Atoms"
      }
    } %}

    <p>The most basic elements of a web system - colors, fonts, grid, etc. These atoms form the basis of this guide.</p>

    <div class="o-inline-list u-margin-top-large">
      <div class="o-inline-list__item u-margin-right">
        {% include "@atoms/logos/site-logo.twig" %}
      </div>

      <div class="o-inline-list__item u-margin-right">
        {% include "@atoms/icons/_icon.twig" with {
          icon: {
            name: 'email'
          }
        } %}
      </div>

      <div class="o-inline-list__item">
        {% include "@atoms/icons/_icon.twig" with {
          icon: {
            name: 'close'
          }
        } %}
      </div>
    </div>
  {% endblock %}
{% endembed %}
</div>

<div class="o-grid__item u-1/1 u-1/2@small u-margin-bottom">
{% embed "@molecules/tiles/tile.twig" with {
  tile: {
    classes: "c-tile--small u-background-color-light-gray"
  }
} %}
  {% block tile_content %}
    {% include "@atoms/typography/headings/h3.twig" with {
      heading: {
        text: "Molecules"
      }
    } %}

    <p>Combinations of two or more atoms that always appear together, e.g. a "share" element or a search box.</p>

    <div class="o-inline-list__item u-margin-top">
      {% include "@molecules/share/share.twig" %}
    </div>
  {% endblock %}
{% endembed %}
</div>

<div class="o-grid__item u-1/1 u-1/2@small u-margin-bottom">
{% embed "@molecules/tiles/tile.twig" with {
  tile: {
    classes: "c-tile--small u-background-color-light-gray"
  }
} %}
  {% block tile_content %}
    {% include "@atoms/typography/headings/h3.twig" with {
      heading: {
        text: "Organisms"
      }
    } %}
    <p>Combinations of molecules that make up a discrete section of a page, e.g. global navigation, or a hero banner.</p>
    <div class="u-margin-top-large">
    {% include "@molecules/tabs/tabs.twig" %}
  </div>
  {% endblock %}
{% endembed %}
</div>

<div class="o-grid__item u-1/1 u-1/2@small u-margin-bottom">
{% embed "@molecules/tiles/tile.twig" with {
  tile: {
    classes: "c-tile--small u-background-color-light-gray"
  }
} %}
  {% block tile_content %}
    {% include "@atoms/typography/headings/h3.twig" with {
      heading: {
        text: "Templates"
      }
    } %}
    Multiple atoms, molecules and organisms that work together to form a discrete page template, e.g. an article or set of search results.
  {% endblock %}
{% endembed %}
</div>

<div class="o-grid__item u-1/1 u-1/2@small u-margin-bottom">
{% embed "@molecules/tiles/tile.twig" with {
  tile: {
    classes: "c-tile--small u-background-color-light-gray"
  }
} %}
  {% block tile_content %}
    {% include "@atoms/typography/headings/h3.twig" with {
      heading: {
        text: "Pages"
      }
    } %}
    The application of real-world content into templates.
  {% endblock %}
{% endembed %}
</div>

</div>