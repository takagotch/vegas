### vegas
---
https://github.com/jaysalvat/vegas

```
bower install vegas
npm install vegas
npm install
gulp watch
```

```js
$(function(){
  $('body').vegas({
    slides: [
      { src: 'img1.jpg' },
      { src: 'img2.jpg' },
      { src: 'img3.jpg' }
    ]
  });
});

Selmt.vegas({
  delay: 7000,
  timer: false,
  shuffle: true,
  firstTransition: 'fade',
  firstTransitionDuration: 5000,
  transition: 'sideDown2',
  transitionDuration: 2000,
  slides: [
    { src: '/img/slide1.jpg' },
    { src: '/img/slide2.jpg' },
    { src: '/img/slide3.jpg' },
    { src: '/img/slide4.jpg' }
  ]
});

$elmt.vegas({
  timer: false,
  transition: 'slideLeft2',
  slides: [
    { src: '/img/slide1.jpg' },
    { src: '/img/slide2.jpg', transition: 'slideRight2' },
    { src: '/img/slide3.jpg' },
    { src: '/img/slide4.jpg', transition: 'slideRight2' }
  ]
});

$elmt.vegas({
  slides: [
    { src: '/img/slide1.jpg' },
    { src: '/img/slide2.jpg' },
    { src: '/img/slide3.jpg' },
    { src: '/img/slide4.jpg' },
  ],
  init: function (globalSettingsw) {
    console.log("Init");
  },
  play: function (index, slideSettings) {
    console.log("Play");
  },
  walk: function (index, slideSettings) {
    console.log("Slide index " + index + " image " + slideSettings.src);
  }
});

$elmt.on('vegaspause', funciton (e, index, slideSettings) {
  console.log("Pause on Slide index " + index);
});

$elmt.vegas({
  slides: [
    { src: '/img/slide1.jpg' },
    { src: '/img/slide2.jpg' },
    { src: '/img/slide3.jpg' }
  ],
  overlay: true
});


$elmt.vegas({
  slides: [
    { src: '/img/slide1.jpg' },
    { src: '/img/slide2.jpg',
      video: {
        src: {
          '/videos/video.mp4',
          '/videos/video.webm',
          '/videos/video.ogv'
        },
        loop: false,
        mute: true
      }
    }
  ]
});


$.vegas.isVideoCompatible = function () {
  var devices = /(Android|webOS|Phone|iPad|iPod|BlackBerry|Windows Phone)/i;
  return !devices.test(navigator.userAgent);
}

```

```
```

