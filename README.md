[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-green.svg)](https://www.webcomponents.org/element/arsnebula/nebula-sidebar-layout)
[![Polymer Version](https://img.shields.io/badge/polymer-v2-blue.svg)](https://www.polymer-project.org)
[![Sauce Labs Build Status](https://img.shields.io/badge/saucelabs-passing-red.svg)](https://saucelabs.com/beta/builds/127a898cf5c24bef91aba79c41e74763)
[![Gitter Chat](https://badges.gitter.im/org.png)](https://gitter.im/arsnebula/webcomponents)
[![Become a Patreon](https://img.shields.io/badge/patreon-support_us-orange.svg)](https://www.patreon.com/arsnebula)

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

## Getting Started

Import the package.

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
nebula-toast {
  color: white;
  background-color: darkred;
}
```

*For more information, see the API documentation.*

## Contributing

We welcome and appreciate feedback from the community. Here are a few ways that you can show your appreciation for this package:

* Give us a **Star on GitHub** from either [webcomponents.org](https://www.webcomponents.org/element/arsnebula/nebula-element-mixin) or directly on [GitHub](https://github.com/arsnebula/nebula-element-mixin).

* Submit a feature request, or a defect report on the [Issues List](https://www.webcomponents.org/element/arsnebula/nebula-element-mixin/issues).

* Become a [Patreon](https://www.patreon.com/arsnebula). It takes a lot of time and effort to develop, document, test and support the elements in our [Nebula Essentials](https://www.webcomponents.org/collection/arsnebula/nebula-essentials) collection. Your financial contribution will help ensure that our entire collection continues to grow and improve.

If you are a developer, and are interested in making a code contribution, consider opening an issue first to describe the change, and discuss with the core repository maintainers. Once you are ready, prepare a pull request:

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## Change Log

See [CHANGELOG](/CHANGELOG.md)

## License

See [LICENSE](/LICENSE.md)