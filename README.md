[![Published on NPM](https://img.shields.io/npm/v/@advanced-rest-client/star-rating.svg)](https://www.npmjs.com/package/@advanced-rest-client/star-rating)

[![Build Status](https://travis-ci.org/advanced-rest-client/star-rating.svg?branch=stage)](https://travis-ci.org/advanced-rest-client/star-rating)

[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/advanced-rest-client/star-rating)

## &lt;star-rating&gt;

A component that renders stars for rating.

```html
<star-rating value="3"></star-rating>
<star-rating value="4" readonly></star-rating>
```

Element can be styled using CSS variables

```html
<star-rating class="theme-blue" value="3"></star-rating>
<style>
.theme-blue {
  --star-rating-unselected-color: #BBDEFB;
  --star-rating-selected-color: #1565C0;
  --star-rating-active-color: #2196F3;
}
</style>
```

### API components

This components is a part of [API components ecosystem](https://elements.advancedrestclient.com/)

## Usage

### Installation
```
npm install --save @advanced-rest-client/star-rating
```

### In an html file

```html
<html>
  <head>
    <script type="module">
      import './node_odules/@advanced-rest-client/star-rating/star-rating.js';
    </script>
  </head>
  <body>
    <star-rating value="2"></star-rating>
  </body>
</html>
```

### In a Polymer 3 element

```js
import {PolymerElement, html} from './node_odules/@polymer/polymer';
import './node_odules/@advanced-rest-client/star-rating/star-rating.js';

class SampleElement extends PolymerElement {
  static get template() {
    return html`
    <star-rating value="2"></star-rating>
    `;
  }
}
customElements.define('sample-element', SampleElement);
```

### Installation

```sh
git clone https://github.com/advanced-rest-client/star-rating
cd api-url-editor
npm install
npm install -g polymer-cli
```

### Running the demo locally

```sh
polymer serve --npm
open http://127.0.0.1:<port>/demo/
```

### Running the tests
```sh
polymer test --npm
```
