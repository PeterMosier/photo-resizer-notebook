# Photo Resizer JupyterLab Notebook

⭐ Note: Github can render/display the Notebook, **but not run it**. Execution happens in Google Colab, and the code has been optimzed to run in Google Colab, decentralized, hence the requirement to upload photos and download results. Early version of this notebook ran on a local machine, and did not require upload/download. The newer versions can be run in the Google Colab cloud from anywhere.

## This JupyterLab Notebook does the following

1. Request the location of the local folder which contains the photos to be processed; these photos are uploaded to Colab
2. One at a time: resize the uploaded file(s) to a **max** size of **1024px wide by 768px** tall
3. Add **copyright text** (hard coded) in top left and bottom right corners of the pic
4. Create **sidecar file**: Extract **EXIF** metadata, if present, and save as a **JSON** file in the **output** directory (**".\webp_resized"**) using the same filename as the photo
5. Save resized photo as .WEBP file (Note: .WEBP format cannot store EXIF metadata) in the **output** directory (**".\webp_resized"**)
6. **ZIP** the .WEBP and .JSON files in **".\webp_resized"** folder and dowload the zip file (**"webp_resized.zip"**) to local machine

This is to prepare resized pics to be uploaded to [UntamedFrames.ca](https://untamedframes.ca)

### Run Option 1: Google Colab
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/PeterMosier/photo-resizer-notebook/blob/main/ImageResizer.ipynb)

### Run Option 2: Binder (not used)
1. Go to [https://mybinder.org](https://mybinder.org)
2. Enter the URL of this repo [https://github.com/PeterMosier/photo-resizer-notebook/](https://github.com/PeterMosier/photo-resizer-notebook/)
3. (Optional) Add a requirements.txt with
   > pillow
   > tqdm
   > exif
4. Click **Launch** and copy the badge code to here in this readme

5. https://github.com/PeterMosier/photo-resizer-notebook/blob/main/ImageResizer.ipynb
