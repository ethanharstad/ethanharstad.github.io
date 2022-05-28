---
title: "Basic LRGB Astrophotography Processing in PixInsight"
draft: true
date: "2022-04-06"
description: ""
tags:
  - "astrophotography"
  - "image processing"
  - "pixinsight"
  - "lrgb"
categories:
  - "astrophotography"
series:
  - "Learning Astrophotography"
featureImage: "image-processing.jpg"
toc: true
---

Blah blah blah

<!--more-->

## Preprocessing

### Subframe Selection

Create weights

### Calibration

Tip: See calibration frames post for process of developing calibration data.

Use ImageCalibration tool once for each set of filter data.
Open Process Explorer > Image Calibration > ImageCalibration
Load Target Frames with Add Files button.
Set an output directory and postfix if desired.
Signal Evaluation and Noise Evaluation are sometimes useful in later stages.
Disable CFA for monochromatic sensors.
ASI2600 (and other cooled CMOS cameras) do not behave well when scaling dark current so dedicated Darks and Flats developed from Dark Flats are used instead.
With dark flat based data, do not use master bias, disable calibration and optimization for master dark, disable calibration for master flat.

### Cosmetic Correction

Cosmetic correction can eliminate remaining defects in calibrated images like hot and cold pixels.

Open Process Explorer > Image Calibration > CosmeticCorrection
Load Target Frames with Add Files button, all frames (L, R, G, B) can be processed together.
Set an output directory and postfix if desired.

You need to use real time preview to see the effects of the process
Open a view of a single frame.
Press Alt+N and drag to select part of the image to preview.
Click the Real Time Preview icon in the bottom left corner of the CosmeticCorrection window (hollow blue circle)

Use Auto Detect
    Hot sigma specifies the how different a pixel can be from its neighbors before being considered a hot pixel
    Cold sigma is the same but for cold pixels
    Lower values are more aggresive and higher numbers are less agressive.
    Use the least agressive setting that eliminates the majority of bad pixels.
    3 is a good starting point for CCDs, 5 is a good start for dedicated astronomy cameras, and 7 is a good start for DSLRs.
Use Master Dark
    Load the master dark file that you used for image calibration.
    Enable both hot and cold pixels thresholds.
    Adjust using the Qty slider first.

### Star Alignment

StarAlignment registers all the images together so that they can be stack.

Select a reference image using the statistics from SFS and your subjective notes from Blink.
Load Target Frames with Add Files button, all frames (L, R, G, B) should be processed together.
The default settings of Projective Transformation as the Registration Model and Register/Matches Images for Working Mode will be fine unless you are building a mosaic.
Distortion Correction is not needed unless you are using an wide field imaging system of 400mm or shorter focal length.
Set an output directory and postfix if desired.

### Integration

#### Superluminance

Integrate L, R, G, B together after removing background gradients.
Compare the SNR of this superluminance image and standard luminance and use the best version.

## Post Processing

### Crop

Inspect all your masters and determine which needs the most cropping.
Begin with that image selected and open the DynamicCrop tool under Geometry.
Drag the crop box over the appropriate portion of the image, being sure to zoom in and verify you're cropping out all the bad data.
Drag the New Instance icon to the workspace desktop to save an instance of these settings.
Click apply to crop your first image, then you can close the DynamicCrop window.
Click and drag the instance you saved onto each of your other images to quickly apply the same settings, then you can delete the saved instance.
