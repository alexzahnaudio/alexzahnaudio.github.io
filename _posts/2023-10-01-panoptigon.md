---
layout: post
title: "Software & Hardware Engineering - Panoptigon"
author: "Alex Zahn"
categories: sample-technical
tags: [sample-technical]
image: panoptigon-full.jpg
---

## Context

In 1971, Mattel, Inc. released the [Optigan](https://en.wikipedia.org/wiki/Optigan) (*Opti*cal Or*gan*) to the world. The predecessor to the Orchestron, it was similar to the Mellotron, but rather than encoding audio tracks onto magnetic tape, it used 12" transparent plastic film discs, inspired by the [optical soundtracks](https://en.wikipedia.org/wiki/Optical_sound) used in the film industry at the time. 57 looping audio tracks, including chord progressions, percussion, and 3 octaves of individual notes on a particular instrument, were printed on the discs as concentric circles, and played via piano keyboard, switches, and buttons.

Long story short, due to mechanical issues and limitations of the optical system, the initial release was a flop, and Mattel lost millions. Despite the imperfections, or maybe in part because of them, it found its way into pop culture (The Clash, Elvis Costello, Third Eye Blind, Kraftwerk, Blur, C418, the Twin Peaks soundtrack...) and became a sort of obscure mythical creature known to niche-audio-gear nerds.

## Rebirth

Most recently, [Quilter Labs](https://www.quilterlabs.com/) (the boutique amp company run by Pat Quilter, founder of QSC), released the [Panoptigon](https://optigan.com/product/panoptigon/) a completely new instrument designed to play Optigan and Orchestron optical discs, with a [plethora of modern features](https://www.youtube.com/watch?v=sX0yEojVHhE), including MIDI control, on-board FX, and multiple drive modes allowing for modulation and fine pitch and speed control. 

In the summer of 2017, I had the opportunity to work at Quilter Labs as an engineering intern. In my time helping with the Panoptigon R&D, I got to experiment and run tests on motor configurations, contribute to the circuit design, do a PCB layout, and work on the firmware run by the on-board microcontroller and DSP unit. I can't go into too much detail about the development, but as the Panoptigon user manual specifically acknowledges the [Spin Semiconductor FV-1](http://www.spinsemi.com/products.html) chip as the onboard DSP effects unit, I can say a bit about that. 

![Panoptigon interface](https://alexzahnaudio.com/assets/img/panoptigon-ui.jpg "Birds-eye view of the Panoptigon")

## Easy DSP FX, Tiny Package

The Spin FV-1 is an awesome little chip. It's got integrated stereo ADCs and DACs, 3 potentiometer inputs for parameter control, and can run up to 16 unique effect programs, 8 of which are built-in, and 8 of which you can program yourself using the "SpinAsm" assembly language (external EEPROM required). You can achieve some great-sounding effects right out of the box, modify the built-in program code to your liking, or experiment with creating your own effects. 

Recently, I was taking a look at the online resources for the Spin FV-1, and saw that Holy City Audio is developing [SpinCAD Designer](https://github.com/HolyCityAudio/SpinCAD-Designer) an open source Java program with a GUI for designing FV-1 patches. My experience was only with the SpinAsm assembly language, so I can't personally attest to SpinCAD Designer's usefulness, but if you choose to experiment with the Spin FV-1 chip for DSP effects on a project of your own (you should; it's kick-ass), SpinCAD Designer seems like it could be a great tool for rapid effects-program prototyping. That said, writing DSP assembly code is a fun challenge of its own... Pick your poison.

![The Spin FV-1 chip](https://alexzahnaudio.com/assets/img/panoptigon-fv-1.jpg "Glorious, powerful, little audio effects chip")

## Appreciations

Working on the Panoptigon was a once-in-a-lifetime experience that I look back on fondly. I was given creative freedom to experiment, and the project touched on mechanical, analog, and digital areas. Not to mention, everyone at Quilter Labs treated me wonderfully. They're really wonderful people, incredibly talented at what they do, and have great taste in pizza. Robert Becker is an absolute wizard.

To cap things off, here's a photo of Rami Jaffee, the Foo Fighters keyboardist, gently caressing the Panoptigon, because I think that's pretty dang cool. Thanks for reading.

![Rami Jaffee with the Panoptigon](https://alexzahnaudio.com/assets/img/panoptigon-rami.jpg "Un-opti-boxing")
