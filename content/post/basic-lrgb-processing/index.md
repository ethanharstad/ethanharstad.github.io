+++
title = "Basic LRGB Astrophotography Processing"
date = "2022-04-06"
description = "A basic LRGB processing workflow with DeepSkyStacker."
tags = [
    "equipment",
    "astrophotography",
    "image processing",
    "deep sky stacker",
    "lrgb",
]
categories = [
    "astrophotography",
]
series = ["Learning Astrophotography"]
featureImage = "image-processing.jpg"
+++

Blah blah blah

<!--more-->

## Preparation

Add all your exposures (lights, darks, bias, flats, dark flats) to DSS and make sure they are all checked.

## Registration

Click "Register checked pictures" - "Register already registered pictures", "Automatic Detection of hot pixels", Uncheck "Stack after registering". Wait...

Sort by image score and mark the highest scored image as reference frame (most likely luminance). Score will have an asterisk next to it.

"Register checked pictures" again with the same settings.

## Stacking

Uncheck all of the RGB frames leaving just the L lights, darks, bias, flats, and dark flats.

"Stack checked pictures" - screenshot

Don't change any settings, "Save picture to file"

Rinse and repeat with R, G, and B

## Post Processing

