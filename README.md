# jwst-img-to-vid
Python scripts to download JWST observations and their associated metadata. For novelty research purposes, we create free animations or videos from deep neural networks.

## Stable Video Diffusion XL Parameters

The following parameters produced 5 second videos on an A100 GPU after pre-editing
the photos for a 576 H x 1024 W pixel image.

 - Frames: 50
 - Frames per second: 10
 - Number of Steps: 60
 - Seed: Random
 - Number of frames decoded at a time: 1
 - Motion bucket id: 200
 - Condition augmentation factor: 0.02

The current notebook supports frames that are in multiples of 25. Length in time is
Frames / Frames per second (5 seconds = 50 frames / 10 fps). Increase in condition
augmentation factor increases "how much can change" in the output video from changing it for the same input.
