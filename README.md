# node-slideshare

This is an easy to use node.js wrapper for the SlideShare REST API.

## Installing

`npm install slideshare`

## Usage

Initialize a SlideShare object with your api key and secret, and call the methods documented in `lib/slideshare.js`.

```js
var SlideShare = require('slideshare');

var ss = new SlideShare('your_api_key', 'your_api_secret');

ss.getSlideshowsByUser('AmitRanjan', { limit: 5, detailed: 0 }, function(result) {
    console.log(result);
});
```
