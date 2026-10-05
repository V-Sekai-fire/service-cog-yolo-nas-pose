# service-cog-yolo-nas-pose

A model container that serves a single-pass person detection and pose estimation network, with an entry point for fine-tuning it.

## What it is for

The prediction endpoint takes an image and returns the detected keypoints as JSON and an annotated image. The training endpoint fine-tunes the pretrained weights on a zipped dataset and returns the new weights.

## Build and run

```sh
just predict path/to/image.jpg
```

This runs the prediction through `cog`, which must be installed.

## Licence

Apache-2.0; see `LICENSE`.
