# Accelerate Editor Networked-AFrame

This is a fork of [networked-aframe/networked-aframe](https://github.com/networked-aframe/networked-aframe) for use with the [Accelerate Editor](https://accelerate-editor.web.app/).

## Change Log

- Any occurance of `document.body` has been replace with `window.top.document.body` to target the parent window.
- `document.location.href` has been replaced with `document.location.origin` has the former didn't seem to get the headers (in [WsEasyRtcAdaper.js](https://github.com/joshmurr/networked-aframe/blob/master/src/adapters/WsEasyRtcAdapter.js#L58). But this is redundant now as we are using the Firebase adapter any way.
