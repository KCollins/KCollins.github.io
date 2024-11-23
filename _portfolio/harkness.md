---
title: "harkness"
excerpt: "A python library for easy VR-compatible 3D data visualization.<br/><img src='/images/image20849.jpg'>"
collection: portfolio
---

[harkness](https://github.com/KCollins/harkness) is a python library for quickly converting pandas dataframes to .ply pointcloud files for viewing in VR.

[![PyPI version](https://badge.fury.io/py/harkness.svg)](https://badge.fury.io/py/harkness) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10223765.svg)](https://doi.org/10.5281/zenodo.10223765)

## Minimum Working Example:
```
# Install harkness if needed:
pip install harkness

# Import libraries
import pandas as pd
from harkness.create_ply import create_ply

# Generate sample data
data = {'X': [1, 2, 3],
        'Y': [4, 5, 6],
        'Z': [7, 8, 9],
        'C': [10, 20, 30]}

df = pd.DataFrame(data)

# Create PLY file
filename = 'example.ply'
create_ply(df, filename, C='C', is_verbose=True)
```

<!-- Import the component -->
<script type="module" src="https://ajax.googleapis.com/ajax/libs/model-viewer/3.3.0/model-viewer.min.js"></script>

<!-- Use it like any other HTML element -->
<model-viewer alt="Neil Armstrong's Spacesuit from the Smithsonian Digitization Programs Office and National Air and Space Museum" src="shared-assets/models/NeilArmstrong.glb" ar environment-image="shared-assets/environments/moon_1k.hdr" poster="shared-assets/models/NeilArmstrong.webp" shadow-intensity="1" camera-controls touch-action="pan-y"></model-viewer>


<!-- <meta name="twitter:card" content="player"/>
<meta name="twitter:site" content="modelviewer"/>
<meta name="twitter:player:width" content="480"/>
<meta name="twitter:player:height" content="480"/>
<meta name="twitter:player" content="https://modelviewer.dev/examples/twitter/player.html?src=https://modelviewer.dev/shared-assets/models/NeilArmstrong.glb&poster=https://modelviewer.dev/shared-assets/models/NeilArmstrongPoster.webp&alt=Neil%20Armstrong%27s%20Spacesuit%20from%20the%20Smithsonian%20Digitization%20Programs%20Office%20and%20National%20Air%20and%20Space%20Museum&environmentImage=https%3A%2F%2Fmodelviewer.dev%2Fshared-assets%2Fenvironments%2Fmoon_1k.hdr"/>
<meta property="og:title" content="3D model-viewer embed"/>
<meta property="og:description" content="Neil Armstrong's Spacesuit from the Smithsonian Digitization Programs Office and National Air and Space Museum"/>
<meta property="og:image" content="https://modelviewer.dev/shared-assets/models/NeilArmstrong.png"/>

<meta http-equiv="refresh" content="0; url='https://modelviewer.dev/'"/> -->
    
