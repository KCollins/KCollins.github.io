---
title: "harkness"
excerpt: "A python library for easy VR-compatible 3D data visualization<br/><img src='/images/image20849.jpg'>"
collection: portfolio
---

harkness is a python library for displaying pandas. 

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
