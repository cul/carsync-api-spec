# CARSYNC-API

API specification describing the responses from the Workflow Manager for the Carnegie Oral History Synchronizer

## Specification Notes

Given an IIIF Manifest for a time-based media resource

Retrieved via HTTP GET from a Workflow Manager

That contains a Range structure describing spans of the media

And contains a link to a WebVTT transcription

And contains a linked AnnotationList that has the OpenAnnotation-editing motivation,

A client should be able to request an AnnotationList that:
* contains an Annotation of the WebVTT transcription in the manifest that links to a working copy of the transcription responding to HTTP GET and PUT
* contains an Annotation of the Range structure in the manifest that links to a working copy of the Range json responding to HTTP GET and PUT

The avalon folder contains IIIF structural examples from Indiana University Digital Libraries.

The carsync folder contains the same example amended with the AnnotationList described above.

## Motivating Use Cases
### OHMS
http://www.oralhistoryonline.org/ohms/

## Motivating Examples
### IU DLib
https://dlib.indiana.edu/iiif_av/lunchroom_manners/lunchroom_manners_v4.json
http://dlib.indiana.edu/iiif_av/lunchroom_manners/lunchroom_manners.vtt

### Digirati Manifests
https://digirati-co-uk.github.io/iiif-av-bl/
https://digirati-co-uk.github.io/iiif-av-bl/data/bl/01_gapless_audio.json

### Avalon IIIF player
https://github.com/avalonmediasystem/avalon-iiif-player/wiki/IIIF-AV-Sample-Manifests
https://github.com/avalonmediasystem/avalon-iiif-player
