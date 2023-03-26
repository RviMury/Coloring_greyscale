# Coloring_greyscale
The model is trained using Autoencoders to colorize the greyscale images to color.
The current model is trined on the images of Green Parks, Sunset and Deserts thus while testing greyscale images of these 3 things should be used
Model will perform very poorly for portraits, household images, etc

### For Downloading traing data images
---python
from bing_image_downloader import downloader
downloader.download('Green Parks', limit=100,  output_dir='dataset',
dadult_filter_off=True, force_replace=False, timeout=60)
----

### Note
- Note Autoencoders require huge computation power and epochs >300 should be used in real life situation
- Also here 100 images of each class is used (green parks, sunsets, deserts). More data will lead to more accuracy.

### Results
The model gives the accuracy of 0.79 at 50 epochs

