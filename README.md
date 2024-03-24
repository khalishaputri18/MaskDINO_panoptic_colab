# **MaskDINO Panoptic Segmentation on Google Colab**

This is my implementation of panoptic segmentation using MaskDINO. The original MaskDINO github available here: https://github.com/IDEA-Research/MaskDINO

What you'll need to prepare:
1. Panoptic segmentation dataset that includes images, COCO Panoptic JSON annotations, and PNG mask annotations.
2. Instance segmentation JSON annotations related to the panoptic segmentation dataset.
3. All datasets and annotations are to be uploaded to Google Drive for easy copy in Google Colab.

All the implementation steps are included in the .ipynb file from installation until the demo.

## Explanation for optional steps

There are several steps that need to be done in order to use custom dataset:
1. Changing `LOAD_TRUNCATED_IMAGES = True` `in ImageFile.py` in PIL.
2. `visualizer.py` and `video_visualizer.py` are used to anticipate unknown classes found in the image/video.
3. Edit the category list in `builtin_meta.py` in detectron2/data/datasets.
4. Change the number of class in the MaskDINO configuration file.


## Result Examples
![furniture15](https://github.com/khalishaputri18/MaskDINO_panoptic_colab/assets/66949610/d195dfc5-788a-4dc3-ad5e-29aaeecda51b)
![furniture11](https://github.com/khalishaputri18/MaskDINO_panoptic_colab/assets/66949610/dbec1090-2d6b-4dcd-8e53-fdfe8e374ed5)
