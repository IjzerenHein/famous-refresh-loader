famous-refresh-loader
==========

Spinning pull to refresh loader for famo.us.

![Screenshot](screenshot.gif)

A spinning pull to refresh loaded that can be used with the famous-flex ScrollView.

## Demos

- [Chat demo](https://rawgit.com/IjzerenHein/famous-flex-chat/master/dist/index.html) ([source](https://github.com/IjzerenHein/famous-flex-chat))


## Getting started

Install using bower or npm:

	bower install famous-refresh-loader

	npm install famous-refresh-loader


## Usage

```javascript
var FlexScrollView = require('famous-flex/ScrollView');
var RefreshLoader = require('famous-refresh-loader/RefreshLoader');

// create scrollview with pull to refresh header
var scrollView = new FlexScrollView({
	pullToRefreshHeader: new RefreshLoader({
		pullToRefresh: true,
		size: [undefined, 60],	// 60px height, to activate refresh pull down at least 120px
		pullToRefreshBackgroundColor: 'white'
	})
});
this.add(scrollView);
```

## Options

The following options are supported by RefreshLoader:

```javascript
var refreshLoader = new RefreshLoader({
	size: [undefined, 100],
	color: '#AAAAAA',			// particle color
    particleCount: 10,			// number of particles
    particleSize: 6,			// size of particle
    rotateVelocity: 0.09,		// rotation velocity
    hideVelocity: 0.05,			// collapse-velocity when hidding
    quickHideVelocity: 0.2,		// quick collapse-velocity when hidding
    pullToRefresh: false,		// enables pull to refresh
    pullToRefreshBackgroundColor: 'white', // color of surfaces which obscures the loader when pulling
    pullToRefreshDirection: 1,	// set to 0 for horizontal pull to refresh
    pullToRefreshFooter: false  // set to true for footer usage
});
```


## Contribute

If you like this project and want to support it, show some love
and give it a star.


## Contact
- 	@IjzerenHein
- 	http://www.gloey.nl
- 	hrutjes@gmail.com

© 2014 - Hein Rutjes
