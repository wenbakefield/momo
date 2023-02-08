# MoMo
A pedalboard-like GUI that allows a user’s mobile device to control a fully customizable Pure Data audio engine.

By connecting an audio input via interface to the mobile device, the system can be used to control a guitar in a simple and intuitive way.

## CHANGES
MoMo v0.9.3 - Changed bandpass filters to bob~, which is an implementation of Moog resonant filter

## INTRODUCTION
This is a demo, packaged for the final project in MUST2431 (Ronald B. Smith) at Northeastern University. 

Each folder contains the elements used in an effect.

The naming conventions are:

* PureData (.pd) files: 
  * <effect>_pedal.pd - the effect abstraction; that is, the "guts"
  * <effect>_top_level_mmp.pd - the patch that interfaces with the MMP GUI made to control the effect
  * <effect>_top_level_pd.pd - the native PD user interface for the effect

* MobMuPlat (.mmp) files:
  * <effect>_top_level.mmp - the MMP GUI 

## MOBILE USE
To use this on a phone:
1. Download the MobMuPlat app.
2. Move all .pd files used in the audio procesing, along with the .mmp files, into the MobMuPlat directory on your mobile device.
3. The files should appear in MobMuPlat (below the example patches).

## REQUIREMENTS
This patch requires Cyclone: https://puredata.info/downloads/cyclone

Debugging mobile GUI requires MobMuPlat: http://danieliglesia.com/mobmuplat/
