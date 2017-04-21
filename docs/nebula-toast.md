# \<nebula-toast\>

`<nebula-toast>` is a custom element to display a toast notification. The notification can be auto-closed after a specified `duration`, or when the user taps or clicks the notification area. The notification can be displayed at the top or the bottom of the screen area.

## Import

```html
<link rel="import" href="/bower_components/nebula-toast/nebula-toast.html"> 
```

## Usage

```html
<nebula-toast
  id="toast"
  position='top'
  duration=5000>
</nebula-toast>
```

Add and configure the element programatically using the `show` method. The element is appended and removed from the `document.body` automatically. The method returns a promise that is resolved once the element closing animation is complete.

```js
const toast = Polymer.Base.create('nebula-toast', {
  text: 'Hello world',
  duration: 5000
})

toast.show().then(function() {
  console.log('The toast has closed')
})
```

## Style

The element can be styled with stardard CSS properties.

```css
nebula-toast {
  color: white;
  background-color: darkred;
}
```

The element also inherits default values from the following global theme styles. If a global theme variable has not been set, it will use the local default.

Custom property | Description | Default
:--- | :--- | :---
`--nebula-ui-border-radius` | The border-radius of the element. | 2px

## API Reference

### Properties

#### opened : Boolean *[reflectToAttribute, notify, value=false]*

Indicates if the element is opened.

#### position : String *[reflectToAttribute, value='bottom']*

Position of the toast (top or bottom).

#### text : String

The text to display.

#### duration : Number *[value=5000]*

The duration (ms) before the element is automatically closed. Set the duration to 0 to close manually.

### Methods

#### show(props) : Promise

Displays the element. If the element does not have a parent, it will be auto appended to `document.body`. A promise is returned that will resolve when the element has been closed.

### Events

#### opened : CustomEvent

Event fired when the opening transition is complete.

#### closed : CustomEvent

Event fired when the closing transition is complete.

### Mixins

#### [Nebula.ElementMixin](https://www.webcomponents.org/element/arsnebula/nebula-element-mixin)