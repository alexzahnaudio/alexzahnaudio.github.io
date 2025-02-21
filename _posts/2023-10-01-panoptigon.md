---
layout: post
title: "Software & Hardware Engineering - Panoptigon"
author: "Alex Zahn"
categories: sample-technical
tags: [sample-technical]
image: panoptigon-full.jpg
---

## Some History

In 1971, Mattel, Inc. released the [Optigan](https://en.wikipedia.org/wiki/Optigan) to the world. It was similar to the Mellotron, but rather than encoding audio tracks onto magnetic tape, it used 12" transparent plastic film discs, inspired by the [optical soundtracks](https://en.wikipedia.org/wiki/Optical_sound) used in the film industry at the time. 57 looping audio tracks, including 3 octaves of individual notes on a particular instrument as well as some percussion and chord progression loops, were printed on the discs as concentric circles, and played via piano keyboard, switches, and buttons.

Long story short, Mattel lost millions, but over time it found its way into pop culture (The Clash, Elvis Costello, Third Eye Blind, Kraftwerk, Blur, C418, the Twin Peaks soundtrack...) and became a sort of obscure mythical beast known only to niche audio gear nerds.

More recently, [Quilter Labs](https://www.quilterlabs.com/) (the boutique amp company headed by Pat Quilter, founder of QSC), released the [Panoptigon](https://optigan.com/product/panoptigon/), a completely new instrument designed to play Optigan and Orchestron optical discs, with [additional modern features](https://www.youtube.com/watch?v=sX0yEojVHhE) like MIDI control, on-board FX, and finely controlled modulation of the servo.

## Okay, Back to Me

Summer of 2017, I had the opportunity to work at Quilter Labs on the Panoptigon R&D. It was a blast, I learned a ton. I look back on it fondly, and thought it might be nice to look back on it fondly here in a way that shares some of what I learned. As the Panoptigon user manual specifically acknowledges the [Spin Semiconductor FV-1](http://www.spinsemi.com/products.html) chip as the onboard DSP effects unit, and I found it strangely delightful to work with, I'm going to hype it up. 

![Panoptigon interface](https://alexzahnaudio.com/assets/img/panoptigon-ui.jpg "Birds-eye view of the Panoptigon")

## Easy DSP FX, Tiny Package

The Spin FV-1 is an awesome little chip. It's got integrated stereo ADCs and DACs, 3 potentiometer inputs for parameter control, and can run up to 16 unique effect programs, 8 of which are built-in, and 8 of which you can program yourself using the "SpinAsm" assembly language (external EEPROM required). You can achieve some great-sounding effects right out of the box, modify the built-in program code to your liking, or experiment with creating your own effects. 

Recently, I was taking a look at the online resources for the Spin FV-1, and saw that Holy City Audio is developing [SpinCAD Designer](https://github.com/HolyCityAudio/SpinCAD-Designer) an open source Java program with a GUI for designing FV-1 patches. My experience was only with the SpinAsm assembly language, so I can't personally attest to SpinCAD Designer's usefulness, but if you choose to experiment with the Spin FV-1 chip for DSP effects on a project of your own (you should; it's kick-ass), SpinCAD Designer seems like it could be a great tool for rapid effects-program prototyping. That said, writing DSP assembly code is a fun challenge of its own... Pick your poison.

![The Spin FV-1 chip](https://alexzahnaudio.com/assets/img/panoptigon-fv-1.jpg "Glorious, powerful, little audio effects chip")

## Some Gratitude

The Panoptigon was a strange, beautiful little thing to work on and it still makes me smile. Everyone on the team at Quilter Labs treated me wonderfully. They're really wonderful people, incredibly talented at what they do, and have great taste in pizza. Robert Becker is a wizard.

To cap things off, because I think it's pretty cool, here's a photo of Rami Jaffee, the Foo Fighters keyboardist, caressing the Panoptigon, gently and lovingly. Thanks for reading.

![Rami Jaffee with the Panoptigon](https://alexzahnaudio.com/assets/img/panoptigon-rami.jpg "Un-opti-boxing")
