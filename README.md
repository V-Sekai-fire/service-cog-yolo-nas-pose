# service-cog-yolo-nas-pose

A model container that serves a single-pass person detection and pose estimation network.

## What it is for

The prediction endpoint takes an image and returns the detected keypoints as JSON and an annotated image. `train.py` is an unfinished training stub and does not train.

## Build and run

```sh
just predict path/to/image.jpg
```

This runs the prediction through `cog` and decodes its output with `jq` and `base64`; all three must be installed.

## Licence

Apache-2.0; see `LICENSE`.
