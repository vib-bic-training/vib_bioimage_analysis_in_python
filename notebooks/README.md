# VIB Bio Image Analysis in Python


## Notebook Structure 

### 0. [Google Colab](https://colab.research.google.com/github/vib-bic-training/vib_bioimage_analysis_in_python/blob/main/notebooks/00_google-colab.ipynb)
**Learning Objectives:**
- Know how to use Google Colab for running Python code in the cloud

### 1. [Image I/O and Visualization](https://colab.research.google.com/github/vib-bic-training/vib_bioimage_analysis_in_python/blob/main/notebooks/01_image-io-and-visualization.ipynb)
**Learning Objectives:**
- Master file I/O operations for various microscopy formats
- Understand image metadata and pixel size information
- Learn effective visualization strategies for multidimensional data

### 2. [Intro to Image Processing](https://colab.research.google.com/github/vib-bic-training/vib_bioimage_analysis_in_python/blob/main/notebooks/02_image-processing.ipynb)
**Learning Objectives:**
- Apply fundamental image processing operations

### 3. [Image Denoising using Deep Learning](https://colab.research.google.com/github/vib-bic-training/vib_bioimage_analysis_in_python/blob/main/notebooks/03_image-denoising-with-N2V2.ipynb)
**Learning Objectives:**
- Understand the principles of self-supervised denoising
- Implement Noise2Void 2 for removing noise without clean reference images
- Learn to train, validate, and apply deep learning models
- Export trained models for future use

### 4. [Automated Cell Segmentation using Deep Learning](https://colab.research.google.com/github/vib-bic-training/vib_bioimage_analysis_in_python/blob/main/notebooks/04_cell-segmentation-with-cellpose.ipynb)
**Learning Objectives:**
- Apply state-of-the-art deep learning for cell segmentation (CellPose)
- Rely mutiple structure (nuclei, cell etc...)
- Extract features from segmented objects (shape and intensity)

### 5. [Intro to Image Processing](https://colab.research.google.com/github/vib-bic-training/vib_bioimage_analysis_in_python/blob/main/notebooks/05_image_processing_with_dask.ipynb)
**Learning Objectives:**
- See how dask array could be used instead of numpy array to process images in chunk for (potentially) large images
- Filter, create mask and label object on chunk

## Run them using Google Colab

All the notebooks are runnable from Google Colab:

Connect to https://colab.research.google.com and signed in

<img width="1215" height="292" alt="image" src="https://github.com/user-attachments/assets/7036ff11-2b9d-4cb3-9ea8-45dce6c5aed4" />

### Open the notebook 

#### Method 1 : click on the link above to open each notebook

If you have a github account, you could open the notebook directly b clicking to link above

#### Method 2 : search for the github notebook

If you have a github account, you could open the notebook directly from github by entering the URL of the github project  https://github.com/vib-bic-training/vib_bioimage_analysis_in_python and search for the notebooks

<img width="889" height="557" alt="image" src="https://github.com/user-attachments/assets/5ed67955-4324-4b64-9efa-03787ddded9d" />

Then click on <img width="29" height="27" alt="image" src="https://github.com/user-attachments/assets/365bba59-2d3a-415b-9100-1ef254002106" /> to open a notebook on your google colab session

<img width="785" height="458" alt="image" src="https://github.com/user-attachments/assets/dd059384-4d0e-4636-98e9-7effc61572d9" />


### Run the notebook 

**Save a copy to your Google Drive to keep changes**

Once you have a notebook open, the first thing to do is to save a copy of it on your Google Drive. This is done by clicking the "Copy to Drive" button at the left in the notebook menu.

<img width="740" height="315" alt="colab_copy" src="https://github.com/user-attachments/assets/46524766-e40d-471b-a406-466adaa49603" />


**Connect to a Python runtime**

Once you have a copy of the notebook on your Google Drive, you can connect it up to a Python runtime. This is done by clicking the "Connect" button in the top right corner of the notebook. This will connect the notebook to a Python runtime, which is a virtual environment that contains the Python interpreter and the libraries that you will need to run your code.

<img width="740" height="315" alt="colab_connect" src="https://github.com/user-attachments/assets/f2508dd7-eaa8-4275-8151-a4f96c284f76" />

If you need a GPU, click on Change run time and select a GPU

<img width="361" height="112" alt="image" src="https://github.com/user-attachments/assets/3ca89807-b394-408b-aaa8-68d59d438d63" />

<br/>


<img width="559" height="515" alt="colab_change_runtime_type_gpu" src="https://github.com/user-attachments/assets/204c3833-7bb7-4110-a6fb-139414fd2b6a" />


**Run the notebook**

A Colab notebook is composed of cells, which can contain code, text, or even images. You can run the notebook entirely by clicking the "Run" button in the top right corner of the notebook. This will execute all the code from start to finish. However, you can also run it cell by cell, or interrupt it if needed without it losing its state. With state, we mean that the notebook will remember the variables and functions that were defined since the last code block was executed.
