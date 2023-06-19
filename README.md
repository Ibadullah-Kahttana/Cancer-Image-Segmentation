# Cancer-Image-Segmentation
In tasks like cancer cell detection, image segmentation is crucial to training deep neural networks. This scenario involves cancer cell images accompanied by JSON files containing polygonal coordinate points that define segmented areas. I developed a solution to map the JSON object onto the original images. 

# Description
> Firstly, we can parse the JSON file to extract the necessary information.
> By reading the JSON file, we can access the array of polygons that represent
> the segmented areas. Each polygon consists of coordinate points defining its boundaries.


## Python Packeges
Install all the below dependencies

```sh

import pandas as pd
import numpy as np
import os
import json
from patchify import patchify
import tifffile as tiff

from PIL import Image,ImageDraw
import matplotlib.pyplot as plt
from matplotlib.patches import Polygon

import cv2

```
## Original Image1
![Ploted JSON coordinates!](https://github.com/Ibadullah-Kahttana/Cancer-Image-Segmentation/assets/97878195/da564fab-ece4-4230-b951-6c107f668d3e)

## Mask image1
![Mask Image!](https://github.com/Ibadullah-Kahttana/Cancer-Image-Segmentation/assets/97878195/c377b238-776e-449e-afe6-437f88d0222f)

## Original Image2
![Ploted JSON coordinates!](https://github.com/Ibadullah-Kahttana/Cancer-Image-Segmentation/assets/97878195/084e69dd-22d6-4ea9-86e1-4527b9cb02b4)

## Mask image2
![Mask Image!](https://github.com/Ibadullah-Kahttana/Cancer-Image-Segmentation/assets/97878195/296dbaf4-74f0-408f-b77f-9579e3f1e35e)
