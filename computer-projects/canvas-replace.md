---
title:  CanvasReplace
permalink:  /computer-projects/canvas-replace/
layout:     default
tags:
 - nodejs
 - web
---

# CanvasReplace

**CanvasReplace** is a web application inspired by [Reddit's r/place](https://en.wikipedia.org/wiki/Place_(Reddit)).
The goal is to have a blank canvas at first, and allow users to place one pixel at a time on it.

This application was first developed by [Al3xCalibur](https://github.com/Al3xCalibur) and [Ardhanaariishvara](https://github.com/Ardhanaariishvara), students at Télécom SudParis for three students clubs : the *Club Code*, *Club Jeux* and *CELL*.

This application has been used by dozens of students during an event week.

Because I later wanted to deploy this application myself, and adapt it to my needs, I have developed one new feature.
This is the ability to define times during which the canvas can be edited, while it is otherwise in a locked state.
During this developement, I have also created a `docker-compose` file.
Because of my needs, I had to expose some more variables with environment variables, so that the app is more adaptable.
I have expanded the short documentation in the `README.md`. 

The source code for this application can be found on [Github](https://github.com/Al3xCalibur/CanvasReplace).

I have developed two other tools using *CanvasReplace*.

## Krokpotin

[Krokpotin](https://github.com/matthias4217/krokpotin) is a simple Discord bot in NodeJS.
One of the module is about the canvas, and contains one command, which fetches data from the canvas to post an image of the current state of the canvas to Discord.

## Canvas Snapshot Capture

[Canvas Snapshot Capture](https://github.com/matthias4217/canvas-snapshot-capture) is another NodeJS application.
Its goal is to capture snapshots of the canvas at regular interval.
This allows to process the picture later into a timelapse.
While such a feature could (and may in the future) be integrated directly onto *CanvasReplace* for more efficiency, I was short on time and this gives the whole a more modular design.
I have created a `docker-compose` file for this project.

*[CELL]: Club de Création d'Expériences Ludiques et Libres
