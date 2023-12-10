# MagicAnimateCraft with Colab

https://github.com/shinshin86/magic-animate-craft-with-colab/assets/8216064/24170e4d-f3c1-4ea0-a6b8-01bc99f38c9f

This project involves utilizing vid2densepose to create custom motion videos based on personal preferences.  
Following the creation of these motion videos, the flow transitions to using MagicAnimate for video production.  
The entire process is facilitated through a Colab environment.

## Start at Google Colab

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](./colab.ipynb)

The Colab note above contains two code cells, each of which, when executed, launches Gradio's web UI.  
Here is a description of each application

**About runtime settings**  
Must be `v100 + high memory` to work properly.

### Vid2DensePose

Upload input images to create motion videos that can be used in MagicAnimate.
The motion video will be forced to resize to 512x512 and the FPS will be changed to 25.
This is because these values are currently the best values for processing in MagicAnimate.

Output file will be placed under `/content/MagicAnimate-hf/demo/output`.

This source code can be found [here](https://github.com/shinshin86/vid2densepose/tree/google-colab).

### MagicAnimate-hf

Motion video created with Vid2DensePose and a single still image can be used to create a video.  
See [MagicAnimate](https://github.com/magic-research/magic-animate) for more information.

This source code can be found [here](https://github.com/shinshin86/magicanimate-hf/tree/magic-animate-craft-with-colab).

## Special Thanks

This project is made possible by these wonderful projects.

* [Vid2DensePose](https://github.com/Flode-Labs/vid2densepose)
* [MagicAnimate](https://github.com/magic-research/magic-animate)
* [magicanimate-hf](https://github.com/camenduru/magicanimate-hf)
