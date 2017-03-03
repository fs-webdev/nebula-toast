[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/arsnebula/nebula-toast)
[![Gitter chat](https://badges.gitter.im/org.png)](https://gitter.im/arsnebula/webcomponents)

[![Build Status](https://saucelabs.com/browser-matrix/arsnebula.svg)](https://saucelabs.com/beta/builds/b44e72b8a48c4042b22fc371e9c52d85)

# \<nebula-toast\>

A web component to display a toast notification.

* Responsive design adapts to screen size
* Can be positioned at the top or the bottom of the screen
* Supports `a11y` for accessability
* Easily styled declaratively or with CSS custom properties
* Can auto-close after a specified duration

> Warning: This element utilizes features of [ECMAScript 2015](http://www.ecma-international.org/ecma-262/6.0/) which may not be supported by all browsers. To ensure support by all browsers, consider using the [Core-js Polyfill](https://github.com/zloirock/core-js).

## Installation

```sh
$ bower install arsnebula/nebula-toast
```

## Usage

Import the package elements:

```html
<link rel="import" href="/bower_components/nebula-toast/nebula-toast.html"> 
```

Add the element.

```html
<nebula-toast
  id="toast"
  position='top'
  background-color="darkred"
  color="white"
  transition-duration="0.5s"
  duration=5000>
</nebula-toast>
```

Add and configure the element programatically using the `show` method. The element is appended and removed from the `document.body` automatically.

```js
var toast = Polymer.Base.create('nebula-toast', {
  text: 'Hello world',
  transition-duration: '0.5s',
  duration: 5000
})

toast.show().then(function() {
  console.log('The toast has closed')
})
```

Style the element.

```css
:host {
  --nebula-toast-color: white;
  --nebula-toast-background-color: darkred;
}
```

*For more information on element properties and methods see the element API documentation.*

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## Change Log

See [CHANGELOG](/CHANGELOG.md)

## License

See [LICENSE](/LICENSE.md)