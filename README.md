# Glasscord-Modules

This is the go-to repository to obtain Glasscord modules.

## What's a module?

A module is nothing other than a user-contributed piece of code that
can modify how Glasscord behaves.

## How do I make one?

Take this as an example:
```js
const { Module } = require("glasstron");

module.exports = class ExampleModule extends Module{

	// Register YOUR CSS properties in this static array!
	static cssProps = ["--example-css-prop"];

	constructor(){
		// Stuff to do when the module is loaded
	}

	windowInit(win){
		// Stuff to do when a new BrowserWindow is spawned
		// 'win' represents the new BrowserWindow object
	}

	update(win, cssProp, value){
		// React to CSS property changes inside of a spawned window
		// 'win' is the window object where the change was detected
		// 'cssProp' is your registered CSS property
		// 'value' is the new value of the property
		// NOTE: The value is NOT parsed! It's ALWAYS a string!
	}
}
```
For further reading, check out the [Module](https://github.com/AryToNeX/Glasscord/blob/master/src/module.js) class
