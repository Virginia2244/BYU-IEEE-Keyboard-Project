# BYU-IEEE-Keyboard-Project
This is the template for both the Ergogen file and the QMK firmware that the BYU IEEE club will be using to create custom keyboards.

## Resources
 - [Ergogen guide by FlatFootFox](https://flatfootfox.com/ergogen-introduction/)
  - [Ergogen Official Website](https://ergogen.xyz/)
  - [Ergogen Auto Layout](https://pashutk.com/ergopad/)
  - [Ergogen Unofficial Website](https://ergogen.cache.works/)
  - [Ergogen Docs](https://docs.ergogen.xyz/)
 - [QMK Firmware](https://qmk.fm/)
 ## Ergogen
Ergogen is a platform that will take the dificult parts of designing a keyboard and gets you 90% of the way there with one web tool. You can use it to design a pcb, case, and face plate. One of the dificult things about it is that it recently updated to v4.0, which has breaking changes to the way it works, but the official docs has been mostly updated but isn't complete. To get a better understaning of ergogen and how to use it well read the [Ergogen guide by FlatFootFox](https://flatfootfox.com/ergogen-introduction/). This is a great introduciton to ergogen and how to use it to make a keyboard.
### Ergogen Auto Layout
This is a great tool to use if you are unsure of what a custom keyboard made for your hands even looks like. After using it you will get an idea of what a custom keyboard for you might look like. This is only supposed to be a visualization tool. When I tried to use it last I couldn't get it to output something Ergogen could read. The export button gave me a csv of the places I touched the screen.
## QMK
QMK is the resource I used to program my keyboard. It is much easier to use than starting programing in C from scratch. That being said starting with the QMK docs can be really difficult as the documentaiton is not friendly to those who are new to it. What I recomend to get started is watch an into to QMK video on youtube, read the getting started seciton in the docs, them run `qmk new-keyboard` and it will walk you through the steps of how to build your firmware. That command will get you through a lot of the dificult early configuration challenges.
## Files
A description of the differnt files in the repository
### config.yaml
 - My Ergogen config file. It is my current code for makeing a keyboard in Ergogen.
### footprints
 - This is where I store any footprints I want to use that are not built into the Ergogen tool. Right now I have changed all of the footprints in some way so I am no longer using any stock Ergogen footprints.
### qmk_firmware
 - This is where I keep the qmk firmware that I use to program the keyboard. It isn't meant to be run in this repo. It is supposed to be copied to a fork of the qmk_firmware branch and ran from there.
### .gitignore
 - I don't want to update the output of my ergogen files so I ignore the output folder.
### .gitmodules
 - I use git modules to include the most up to date version of different footprints in my project.
### points_demo.yaml
 - This file is the yaml for the pointmap I made live in the IEEE club. It is a good example of using metatdata and points and a rather poor example of using units. It is not perfect and should not be used as the basis of a keyboard but rather an example of how to use the funcitons and paramaters of Ergogen.
### outlines_demo.yaml
 - This is another file generated from a live demonstration of how to use outlines in Ergogen. It has examples of many of the basic features of an ergogen 