# CloudCannon Vanilla Live Editing Demo

This repo serves as an example of implementing live editing on CloudCannon using vanilla JavaScript.

In the `index.html` layout the relevant attributes are:
- `data-cms-bind` attributes control [CloudCannon Visual Data Bindings](https://cloudcannon.com/documentation/articles/what-are-visual-data-bindings/), which drives the clickable panels in the CloudCannon Visual Editor. This is an out-of-the-box CloudCannon feature _(not specific to this site)_.
- `data-custom-live-editing` attributes are specific to this site, and are used by our `custom-live.js` script to implement the re-rendering side of a live editing workflow.

The `custom-live.js` file accepts front matter update events from CloudCannon, and applies them to the page based on our `data-custom-live-editing` attributes.
