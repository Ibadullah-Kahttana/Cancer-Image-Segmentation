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
## Original Images
![Cancer Image!]()
## Ploted JSON coordinates
## Mask images
