# lazyLoadImages

Simple jQuery plugin to lazy load images visible in the viewport and load images that become visible in the viewport.

## Suggested HTML Markup

```no-highlight
<a href='/'>
  <div data-lazy-load='true' data-src='http://www.example.com/example.png' data-alt='An Example Image'></div>
</a>
```

## Initializing the plugin

```javascript
$(document).ready(function(){
  $("[data-lazy-load]").lazyLoadImages();
});
```

## Notes

The element that you store your information should be the only child of another element (a, span, whatever).  We require a wrapper element that we'll replace the html w/ the lazy loaded image.

## Data Attributes

This plugin accepts the following data attributes that will get passed on to the appropriate attribute in the image:

* data-src
* data-alt
* data-title
