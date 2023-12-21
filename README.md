# Realtime Color Detection Web App

Welcome to our Realtime Color Detection Web App! This application enables color detection in images using Python, OpenCV, and Flask. It's deployed on Google App Engine and uses Firebase for image storage and retrieval.

## Project Overview

Our passion drove us to create a user-friendly web app allowing users to upload an image and retrieve color names by clicking on any pixel.

* **Web App**: [Realtime Color Detection Web App](https://dogwood-sprite-408814.ue.r.appspot.com/)

## Color Detection Algorithm

Utilizing OpenCV, images are processed and converted to the HSV color space, offering a more intuitive representation than RGB. The algorithm matches each pixel to the closest color using predefined HSV values. This comparison is done using the Euclidean distance formula.

## Color Dataset

We leverage a CSV file containing names, hex codes, and RGB values for 865 colors. The RGB values are converted to HSV using `cv2.cvtColor`. The dataset simplifies color identification and can be downloaded [here](#).

## Requirements

To run the app locally, ensure the following packages are installed:

- Python 3.9 or higher
- Flask==1.1.2
- numpy==1.19.5
- opencv-python==4.5.1.48
- gunicorn==20.1.0
- Jinja2==2.11.3
- MarkupSafe==2.1.3

# Install these using `pip`:
```shell
pip install -r requirements.txt
```
# Usage
To run the app locally:
```shell
python app.py
```
Then, open your browser at http://localhost:5000/.

