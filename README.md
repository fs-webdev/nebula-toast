[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://beta.webcomponents.org/element/arsnebula/nebula-toast)
# \<nebula-toast\>

A web component to display a toast notification.

## Installation

```
$ bower install arsnebula/nebula-toast
```

## Usage

Import the package elements:

```
<link rel="import" href="bower_components/nebula-toast/nebula-toast.html"> 
```

Add and configure the element declaratively:

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

or add and configure the element programatically using the `show` method. The element is auto-appeneded and removed from the `document.body` if not done manually.

```js
var toast = document.createElement('nebula-toast')

toast.show({
  text: 'Hello world',
  backgroundColor: 'black',
  color: 'yellow',
  transition-duration: '0.5s',
  duration: 5000
}).then(function() {
  console.log('The toast has closed')
})
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