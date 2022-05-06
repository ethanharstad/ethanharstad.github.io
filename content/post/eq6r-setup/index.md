---
title: "Setting up the Sky-Watcher EQ6-R"
date: "2022-03-26"
description: "Setting up the Sky-Watcher EQ6-R Pro equatorial telescope mount"
tags:
  - "equipment"
  - "astrophotography"
  - "eq6r"
categories:
  - "astrophotography"
series: "Learning Astrophotography"
featureImage: "astrophoto_rig.jpg"
featureImageAlt: "Alt text"
featureImageCap: "Image caption"
thumbnail: "astrophoto_rig-thumb.jpg"
featured: true
summary: "The Sky-Watcher EQ6-R Pro is a German Equatorial telescope mount with many improvements over other mounts that make it ideal for astrophotography."
---

The [Sky-Watcher EQ6-R Pro](https://www.skywatcherusa.com/products/eq6-r-pro) is a German Equatorial telescope mount with many improvements over other mounts that make it ideal for astrophotography.

- Payload: 44lbs / 20kg
- Mount Weight: 38lb / 17.2kg
- Tripod Weight: 16.5lb / 7.5kg
- Permanent periodic error correction
- Belt driven axes
- Vixen and Losmandy compatible saddle plate

## Assembly

It's just a tripod, it is pretty straightforward to set up.

1. Spread out the tripod legs and set the tripod on roughly level ground with the stud aligned with North.
If the ground is soft, it will help to put something underneath the tripod feet or fit some large washers onto the feet.

2. Unlock the legs and raise the tripod to your desired observing height (bear in mind that the more the legs are extended, the more susceptible the mount is to vibration).
Lock the northern leg and raise/lower the other two legs to set the North/South level.
Lock one of the remaining legs and raise/lower the remaining unlocked leg to set the East/West level.

3. Loosen the two azimuth adjusting bolts on the mount head and set the mount on the tripod, aligning the stud with the gap between the azimuth bolts.
Slightly tighten the two azimuth adjusting bolts to gently hold the mount in place.

4. Support the mount with one hand and push the central locking shaft up into the mount, turning the shaft counter-clockwise to secure the mount to the tripod.

5. Slide the accessory tray up along the locking shaft and secure the tray with the locking washer and bolt.
The accessory tray is required to ensure the tripod legs remain rigid throughout observing.
Attach the hand controller bracket to a tripod leg if desired.

6. Loosen the knob securing the counterweight shaft and extend it, re-tighten the knob to secure the shaft again.
Remove the countweight shaft cap and install the desired counterweights and/or shaft extension before replace the shaft cap for safety.

## Mounting and Balancing

Proper balancing of your telescope reduces the work the mount has to do which increases tracking accuracy and increases the life of your mount.

1. Release the R.A. axis clutch and set the position so that the counterweight shaft is pointing straight down before resecuring the clutch.
Release the Declination axis clutch and set the axis position so that the saddle knobs are pointing up and the dovetail groove is level before resecuring the clutch.

2. Loosen the saddle knobs and seat the telescope dovetail into the saddle plate, tightening the two knobs to secure the telescope.

3. Loosen the R.A. axis clutch and rotate the axis until the counterweight shaft is parallel to the ground, resecure the clutch.
Loosen the Declination axis clutch and rotate the axis until the telescope is parallel to the ground, resecure the clutch.

4. Hold the telescope with one hand and carefully loosen the Declination axis clutch.
Adjust the telescope position forward/backward in the saddle until the mount is able to remain stationary without support.
Verify that the mount is able to remain stationary in multiple orientations.

5. Hold the counterweight shaft with one hand and carefully loosen the R.A. axis clutch.
Move the counterweights along the counterweight shaft until the mount is able to remain stationary without support.
Tighten the counterweights and verify that the mount is able to remain stationary in multiple orientations.

5. Loosen the R.A. axis clutch and rotate the axis until the counterweight shaft is pointing straight down, resecure the clutch.
Loosen the Declination axis clutch and rotate the axis until the telescope is parallel to the ground, resecure the clutch.
This is the "Park" and "Home" position of the mount.

{{< notice tip "Tip" >}}
You may get better guiding performance if you set your mount up to be "East Heavy", that is with the counterweight side being slightly heavier before meridian flip.
This can help to reduce the effect of backlash induced oscillations in the mount.
{{< /notice >}}

## Alignment

Your equatorial mount needs to be aligned to the axis of rotation of the Earth in order to effectively track celestial objects.

### Preparation

{{< notice tip "Tip" >}}
It is strongly recommended to mount and balance your telescope before performing polar alignment.
{{< /notice >}}

1. When you set up your tripod you should have performed a rough alignment with the North Pole.
If you did not, now is the time to do it (and remember how hard it is with a fully loaded mount and do it ahead of time next time).

2. You also should have already roughly set the R.A. axis's elevation to your latitude, if you didn't, go do that now (same story).

3. Remove the polar scope caps and then loosen the declination axis clutch and rotate the axis until the hole in the R.A. axis shaft aligns with the polar scope.

4. Turn on the mount to illuminate the the polar scope and verify you can see Polaris inside the scope. If you cannot see Polaris inside the field of view, verify you have aligned the mount with the North Pole and set the R.A. axis elevation to your latitude. If the stars appear blurry, turn the knurled ring on the eyepiece to focus.

### Polar Scope Alignment

WHen you first purchase the mount or if you have travelled or not used the mount in a while you need to calibrate the polar scope to the R.A. axis before you can use it to perform polar alignment.
You do not need to do this every time you use the mount (though it doesn't hurt if you have the time).

1. Select a far-away, fixed object and adjust the azimuth and elevation adjustment bolts to center the polar scope reticle over this object.

2. Loosen the R.A. axis clutch before turning the axis through half a turn (look at the dial to do this accurately) and then tightening the axis clutch again.

3. If the object remains at the center of the reticle then the scope is calibrated and your job is done.
If the object moved, use the three adjustment screws on the polar scope to move the object halfway back to the center of the reticle.

{{< notice warning "Warning" >}}
Only loosen one of the screws 1/4 turn before tightening the other two screws to prevent disengaging or damaging the pattern plate.
{{< /notice >}}

4. Repeat steps 1 through 3 a few times until the object stays at the center of the reticle.

{{< notice note "Note" >}}
If the pattern plate becomes disengaged, remove the eyepiece by turning the knurled ring counterclockwise and re-engage the pattern plate.
{{< /notice >}}

### Polar Alignment

1. Find the correct position of Polaris for your current location and time by waiting for the "Polaris Position in P.Scope=HH:MM" message after the SynScan controller finishished initializing or by using app such as [Polar Finder](https://play.google.com/store/apps/details?id=com.techhead.polarfinder&hl=en).

2. Visualize the reticle circle as a clock face and move Polaris to the indicated position.
Loosen one of the azimuth or elevation knobs and then tighten the opposite knob to move Polaris.
Do not try to use both axis at once and do not over tighten the knobs or you may crack your mount or the adjustment bolts.

### GoTo Alignment

1. Setup home position...

2. Initialize the hand control

## Observing!

Get out there and observe!

## Resources

- [EQ6-R Manual](eq6-r_manual.pdf)
- [SynScan Manual](synscan_manual.pdf)
