requirejs-youtube-player
========================
[![Build Status](https://travis-ci.org/thomaswelton/requirejs-youtube-player.png)](https://travis-ci.org/thomaswelton/requirejs-youtube-player)
[![Dependency Status](https://david-dm.org/thomaswelton/requirejs-youtube-player.png)](https://david-dm.org/thomaswelton/requirejs-youtube-player)
[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/thomaswelton/requirejs-youtube-player/trend.png)](https://bitdeli.com/free "Bitdeli Badge")

AMD compatible helper for loading the Youtube API and injecting videos

Create a new YoutubePlayer that replaces the `element` using a `videoId` and either passing in `dimensions` or allowing CSS values to be used

``new YouTubePlayer(element, videoId, dimensions)``

```javascript
var video1 = new YouTubePlayer( $('player1'), '_OBlgSz8sSM', { width: 200, height:200 } );
var video2 = new YouTubePlayer( $('player2'), 'J---aiyznGQ', { width: 500 } );
var video3 = new YouTubePlayer( $('player3'), 'FzRH3iTQPrk' );
```

Adding events

```javascript
video1.addEvent('onPlay', function(){
	// Video fired YT.PlayerState.PLAYING
});
```

Supported events
- onEnd
- onPlay
- onPause
- onBuffer
- onCued
