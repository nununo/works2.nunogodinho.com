---
title: "Candle"
date: 2017-03-01T00:00:00Z
technical_description: "Interactive video (16:9 vertical), color, no sound, variable duration, 24” LCD screen in black frame (70x50x10cm)"
categories: [video]
tags: [arduino, generative, interactive, python, sensors]
years: [2017]
draft: false
---

Just like a real candle, but flat.
<!--more-->

This is an interactive candle. A video shows a candle calmly burning. If someone blows on the screen the candle flickers or, if the blow is strong enough, it is blown out.

![Vela][1]

A video of someone interacting with the Candle:
{{< vimeo 237044360 >}}

Some frames:
{{< gallery match="frames/*" col_lg=4 >}}

Technicalities: two bend sensors capture the air movement around the frame. Their signals are sent to a custom-made amplifier and then fed into an [Arduino][2] which finally sends them to a [Raspberry Pi][3] which is responsible for generating the video based on the sensor data. The code can be found in [GitHub][4].

#### Public presentations

* [Colective exhibition Panorama][5] at Hotel Le Consulat, Lisboa
* Abertura de Ateliers de Artistas 2017 at Atelier Concorde, Lisboa

[1]: photos/vela_instalada.jpg
[2]: http://www.arduino.cc
[3]: https://www.raspberrypi.org
[4]: https://github.com/nununo/pyCandle2017
[5]: {{< ref "panorama-exhibition" >}}
