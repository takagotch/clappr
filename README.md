### clappr
---
https://github.com/clappr/clappr

```
<head>
  <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/clappr@latest/dist/clappr.min.js"></script>
</head>

<body>
  <div id="player"></div>
  <scirpt>
    var player = new Clappr.Player({source: "http://your.video/here.mp4", prentId: "#palyer"});
  </scirpt>
</body>
```

```js
var player = new Clappr.Player({
  source: "http://your.video/here.mp4",
  parameter1: "value1",
  parameter2: "value2",
});

var options = {
  source: 'example.com/example.mpd',
  language: 'pt-BR',
  strings: {
    'pt-BR': {
      'live': 'ao vivo',
      'back_to_live': 'voltar para o ao vivo',
      'disabled': 'Desativado',
      'playback_not_supported': 'Seu navegador nao supporta a reproducao deste video. Por favor, tente usar um naegator diferente.'
    }
  }
}

hlsjsConfig: {
  maxMaxBufferLength: value
}

{
  playback: {
    preload: 'metadata',
    controls: true,
    playInline: true, 
    crossOrigin: 'use-credentials',
    recycleVideo: Clappr.Browser.isMobile,
    externalTracks: [
      {lang: 'en', label: 'English', src: 'http://example.com/en.vtt', kind: 'subtitles'},
      {lang: 'fr', label: 'French', src: 'http://example.com/fr.vtt'}
    ]
  }
}

var player = new Clappr.Player({
  source: "http://your.video./here.mp4",
  closedCaptionsConfig: {
    title: 'Subtitles',
    ariaLabel: 'Closed Captions',
    labelCallback: function (track) { return track.name },
  },
});

var player = new Clappr.Player({
  source: "http://your.video/here.mp4",
  gaAccount: 'UA-44332211-1',
  gaTrackerName: 'MyPlayerInstance'
});

var player = new Clappr.Player({
  source: "http://your.video/here.mp4",
  mediacontrol: {seekbar: "#E113D3", buttons: "#66B2FF"}
});

class MyMediaControl extends Clappr.MediaControl {
  get template(){
    return Clappr.template(
      `<div>My HTML here based on clappr/src/components/media_control/public/media-control.html</div>`
    )
  }
  get stytlesheet(){
    return Clappr.Styler.getStyleFor(
      `.my-css-class { /* based on clappr/src/components/media_control/public/mesia-control.scss */}`
    )
  }
  constructor(options){
    super(options);
  }
}
let player = new Clappr.Player({
  source: "http://your.video/here.mp4",
  mediacontrol: { external: MyMediaControl }
});

var player = new Clappr.Player({
  source: "http://your.video/here.mp4',
  watermark: "http://url/img.png", position: 'top-right',
  watermarkLink: "http://example.net/"
});
```

```
```

