# ITP Help Site Wordpress
The ITP Help Site was redeveloped using the Wordpress platform to address a number of accessibility issues presented by Google Site. It is based on the Twenty Seventeen and uses components from the [A11Y Style Guide](https://a11y-style-guide.com/style-guide/ "A11Y website") for extended functionality.

## Plugins
* Simple Calendar - For Google Calendar
* Simple Custom CSS & JS - Edit css and js 
* WP File Manager - Upload files

## Creating Additional Accordion Menu Items
The accordions use the [A11Y Style Guide Library](https://a11y-style-guide.com/style-guide/section-navigation.html#kssref-navigation-accordion "A11Y  website"). These buttons are formatted to be tab-able and contain aria labels. Accordions must be coded in.

```
<section class="accordion-section">
  <div class="accordion" role="presentation">
    <div class="js-accordion__panel">
      <h3 class="accordion__heading">
      <button class="accordion__trigger" aria-controls="accordion__content_1" aria-expanded="false" tabindex="0" id="accordion__title_1" aria-selected="false">I’m tall when I’m young and I’m short when I’m old. What am I?
      </button>
      </h3>
      <div class="accordion__content" id="accordion__content_1" role="region" aria-hidden="true" aria-labelledby="accordion__title_1">
        <p>A candle</p>
      </div>
    </div>
    <div class="js-accordion__panel">
      <h3 class="accordion__heading">
      <button class="accordion__trigger" aria-controls="accordion__content_2" aria-expanded="false" tabindex="0" id="accordion__title_2" aria-selected="false">Which weighs more, a pound of feathers or a pound of bricks?
      </button>
      </h3>
      <div class="accordion__content" id="accordion__content_2" role="region" aria-hidden="true" aria-labelledby="accordion__title_2">
        <p>Neither, they both weigh one pound.</p>
      </div>
    </div>
    <div class="js-accordion__panel">
      <h3 class="accordion__heading">
      <button class="accordion__trigger" aria-controls="accordion__content_3" aria-expanded="false" tabindex="0" id="accordion__title_3" aria-selected="false">The more you take, the more you leave behind. What are they?
      </button>
      </h3>
      <div class="accordion__content" id="accordion__content_3" role="region" aria-hidden="true" aria-labelledby="accordion__title_3">
        <p>Footprints.</p>
      </div>
    </div>
  </div>
</section>
```
