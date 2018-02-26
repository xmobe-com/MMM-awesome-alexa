[![Chat on Gitter][gitter-image]][gitter-url]
[![Dependency Status][gemnasium-image]][gemnasium-url]
[![dependencies Status][daviddm-image]][daviddm-url]
[![Build Status][travis-image]][travis-url]
[![Greenkeeper badge][greenkeeper-image]][greenkeeper-url]

<p align="center">
   <img src="https://user-images.githubusercontent.com/2917613/28090232-861702b0-6683-11e7-8379-1347e01c9411.png" height="300">
<p>

# MMM-awesome-alexa

> A hands free Alexa module for the Magic Mirror, which is activated when you say 'Alexa'.
> At the moment, this only works for MacOS and Ubuntu. Raspberry Pi has experimental support, it works when I tried it, but please try yourself and let us know on Gitter!

## Installing

1. First you have to setup your speakers and microphone correctly: [Audio setup](docs/AudioSetup.md)

2. After you have done audio setup you can install Awesome Alexa module to your MagicMirror: [Installation](docs/Installation.md)

## Usage

Boot up `Magic Mirror` and say "Alexa, what time is it?", or "Alexa, tell me a joke" 😊.

**Note:** If you are using Raspberry Pi, you most likely will experience a `snowboy` issue. Please go to the [Troubleshoot](#troubleshoot) section down below

## What to do next?

So you have got it this far and very happy with your working Alexa-enabled MagicMirror. You can then change your time/location; by default, the Alexa is based in Seattle: https://github.com/alexa/alexa-avs-sample-app/issues/222

# Features

* Wake Word support
* Custom Wake Word
* Very easy set up
* Easy config tool
* All-in-one solution.
* Visualization

## Supported Wake Words

* Alexa
* Smart Mirror
* Snowboy

### Coming Soon

* Computer
* Jarvis

# Contribution Guide

Want to contribute? Read the guide here: https://github.com/dolanmiu/MMM-awesome-alexa/wiki/Contribution-Guide

# Troubleshoot

First check if your mic works by typing in:

```bash
rec t.wav
```

If the above command doesn't work, please fix that before continuing. [Here is a link to help you (Raspberry pi)](https://www.raspberrypi.org/forums/viewtopic.php?t=13088&p=332703)

## Snowboy problems

If you are getting an error related to `snowboy`, run this command inside the `MMM-awesome-alexa` folder:

```bash
$ npm run electron-rebuild
```

If that still doesn't work, use node `6.10.x`, and then re-run the above command. There was this [issue about node `7.0.0`](https://github.com/Kitt-AI/snowboy/issues/117), and [node `8.0.0`](https://github.com/Kitt-AI/snowboy/issues/212).

### Still doesn't work

Follow `snowboy`'s official guide on how to recompile their package:
https://github.com/Kitt-AI/snowboy#compile-a-node-addon

---

Made with 💖 by Dolan. Huge thanks to [henrikra](https://github.com/henrikra/) for his contributions to this project!

[gitter-image]: https://badges.gitter.im/dolanmiu/awesome-alexa.svg
[gitter-url]: https://gitter.im/awesome-alexa/Lobby
[gemnasium-image]: https://gemnasium.com/badges/github.com/dolanmiu/MMM-awesome-alexa.svg
[gemnasium-url]: https://gemnasium.com/github.com/dolanmiu/MMM-awesome-alexa
[travis-image]: https://travis-ci.org/dolanmiu/MMM-awesome-alexa.svg?branch=master
[travis-url]: https://travis-ci.org/dolanmiu/MMM-awesome-alexa
[daviddm-image]: https://david-dm.org/dolanmiu/MMM-awesome-alexa/status.svg
[daviddm-url]: https://david-dm.org/dolanmiu/MMM-awesome-alexa
[greenkeeper-image]: https://badges.greenkeeper.io/dolanmiu/MMM-awesome-alexa.svg
[greenkeeper-url]: https://greenkeeper.io/
