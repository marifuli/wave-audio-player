# HTML5 wave-audio-player

![Image demo](https://github.com/marifuli/wave-audio-player/raw/master/preview.png)

## NPM install :
```
npm i wave-audio-player
```

### Import ans use: 
```
<wave-audio-player
    class="first"
    src="/samples/file.mp3" 
    wave-width="200"
    wave-height="40"
    onEnded="eventFired"
    onError="eventFired"
    onLoadedmetadata="eventFired"
    onCanplay="eventFired"
    onCanplaythrough="eventFired"
    onDurationchange="eventFired"
    onEmptied="eventFired"
    onLoadeddata="eventFired"
    onPause="eventFired"
    onPlay="eventFired"
    onPlaying="eventFired"
    onRatechange="eventFired"
    onSeeked="eventFired"
    onSeeking="eventFired"
    onStalled="eventFired"
    onSuspend="eventFired"
    onTimeupdate="eventFired"
    onVolumechange="eventFired"
    onWaiting="eventFired"
></wave-audio-player>

<h3>Animation</h3>
<wave-audio-player src="hello_world.ogg" wave-width="200" wave-height="40" wave-options='{"animation":true,"samples":50}'></wave-audio-player>

<h3>Customized Attributes</h3>
<wave-audio-player
    src="hello_world.ogg"
    wave-width="200"
    wave-height="40"
    color="#55007f"
    wave-color="#55007f"
    wave-progress-color="#ff00ff"
    wave-slider="#ffaaff"
    wave-options='{"samples":40,"type":"steps","width":192,"height":40}'
></wave-audio-player>

<wave-audio-player
    src="hello_world.ogg"
    wave-width="200"
    wave-height="80"
    color="#00aa7f"
    wave-color="#00aa7f"
    wave-progress-color="#aaff00"
    wave-slider="#00aa00"
    wave-options='{"samples":50,"type":"steps","paths":[{"d":"V","sy":0,"x":0,"ey":100},{"d":"A","sx":0,"sy":100,"ex":100,"ey":100,"rx":10,"ry":10,"angle":180,"arc":1,"sweep":1},{"d":"V","sy":0,"x":100,"ey":100}]}'
></wave-audio-player>
```

### Attributes
Name | Required | Type | Description
--- | --- | --- | --- 
src | True | audio file | Source path to audio file
wave_width | True | Integer | Width of the Waves. (Not responsive, Also remember that the buttons and the timing strings will take extra ~250px. For example, if(container === 500px) => wave_width = 500 - 250 = 250  )
wave_height | True | Integer | Height of the waves (Not Responsive)
wave_type | False | String | Type of wave. (Not working yet)
wave_options | False | Object | Set settings for the waves (Not working yet)


Check [MDN Doc](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/audio) for all the events.

### Main project: 
Customized and Advanced version of [wave-path-audio-player](https://github.com/jerosoler/wave-audio-path-player)