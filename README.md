[![Published on NPM](https://img.shields.io/npm/v/@polymer/paper-fab.svg)](https://www.npmjs.com/package/@polymer/paper-fab)
[![Build status](https://travis-ci.org/PolymerElements/paper-fab.svg?branch=master)](https://travis-ci.org/PolymerElements/paper-fab)
[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://webcomponents.org/element/@polymer/paper-fab)

## &lt;paper-fab&gt;
`paper-fab` is a floating action button. It contains an image placed in the center and
comes in two sizes: regular size and a smaller size by applying the attribute `mini`. When
the user touches the button, a ripple effect emanates from the center of the button.

See: [Documentation](https://www.webcomponents.org/element/@polymer/paper-fab),
  [Demo](https://www.webcomponents.org/element/@polymer/paper-fab/demo/demo/index.html).

## Usage

### Installation
```
npm install --save @polymer/paper-fab
```

### In an html file
```html
<html>
  <head>
    <script type="module">
      import '@polymer/paper-fab/paper-fab.js';
      import '@polymer/iron-icons/iron-icons.html';
    </script>
  </head>
  <body>
    <paper-fab icon="favorite"></paper-fab>
    <paper-fab label="😻"></paper-fab>
  </body>
</html>
```

### In a Polymer 3 element
```js
import {PolymerElement, html} from '@polymer/polymer';
import '@polymer/paper-fab/paper-fab.js';
import '@polymer/iron-icons/iron-icons.html';

class SampleElement extends PolymerElement {
  static get template() {
    return html`
    <paper-fab icon="favorite"></paper-fab>
    <paper-fab label="😻"></paper-fab>
    `;
  }
}
customElements.define('sample-element', SampleElement);
```

## Contributing
If you want to send a PR to this element, here are
the instructions for running the tests and demo locally:

### Installation
```sh
git clone https://github.com/PolymerElements/paper-fab
cd paper-fab
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
