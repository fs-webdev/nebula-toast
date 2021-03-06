# Change Log

## [v2.0.1](https://github.com/arsnebula/nebula-toast/releases/tag/v2.0.1) (2017-05-22)

- Refactoring from transitions to animation to support 'display:none' when closed.
- Added animate attribute to allow styling animation easier.
- Added CSS variables for color and background color.
- Remove manual documentation and updated inline comments for API documentation generation.

## [v2.0.0](https://github.com/arsnebula/nebula-toast/releases/tag/v2.0.0) (2017-04-21)

- Upgraded to Polymer v2 ES2015 class-style element.

## [v1.1.1](https://github.com/arsnebula/nebula-toast/releases/tag/v1.1.1) (2017-03-02)

- Minor fixes and tweaks to demo.
- Fixed bug with keydown event handler naming.

## [v1.1.0](https://github.com/arsnebula/nebula-toast/releases/tag/v1.1.0) (2017-03-02)

- Removed style attributes behavior. **BREAKING**
- Added support for global style attributes.
- Removed dependency on iron-a11y-announcer.
- Added promise-polyfill to demo and test pages (remove core.js).
- Updated test configuration for parameter-driven testing.

## [v1.0.4](https://github.com/arsnebula/nebula-toast/releases/tag/v1.0.4) (2017-01-31)

- Removed dependency on iron-a11y-keys-behavior.
- Added support for style attributes behavior.
- Changed test configuration to include IE/Edge and ES5 compatability.
- Fixed method declaration issue with IE/Edge.
- Added test index for test suites.
- Added tests for polyfill and native shadow dom.
- Added test configuration for Sauce Labs.
- Added Sauce Labs badges to README.

## [v1.0.3](https://github.com/arsnebula/nebula-toast/releases/tag/v1.0.3) (2017-01-19)

- Fixed missing import

## [v1.0.2](https://github.com/arsnebula/nebula-toast/releases/tag/v1.0.2) (2017-01-19)

- Added `a11y` accessability support for keyboard and screen readers

## [v1.0.1](https://github.com/arsnebula/nebula-toast/releases/tag/v1.0.1) (2017-01-19)

- Added `transitionDuration` property to declaratively set the animation speed
- Changed style property updates to use single observer handler
- Changed font styles to use system font/size
- Added z-index style to force top of stacking order
- Changed show method to auto-append/remove element from document
- Added demo for dynamically creating/showing the element

## [v1.0.0](https://github.com/arsnebula/nebula-toast/releases/tag/v1.0.0) (2017-01-18)

- Added initial release code