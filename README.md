# MADLab DICOM Workshop (2025)
This repository includes download instructions and supplementary .STL files for the DICOM to 3D file processing workshop provided by MADLab, at U of T in Summer of 2025.
Please follow the steps below to download the relevant DICOM files needed for the workshop. 

# Instructions on Downloading Root Files
This guide provides step-by-step instructions for downloading the software needed and root files using the Imaging Data Commons (IDC) platform.

## Step 1: Relevant Links
Please bookmark the following links:
- [Imaging Data Commons Portal for filtering anonymized patient DICOM files](https://portal.imaging.datacommons.cancer.gov/explore/)
- [IDC GitHub Repository for documentations about downloading from IDC](https://github.com/ImagingDataCommons/idc-index)
- [3D Slicer Software for converting DICOM images into 3D files](https://download.slicer.org/)
- [MeshMixer Software for repairing and refining 3D files](https://apps.autodesk.com/FUSION/en/Detail/Index?id=4108920185261935100)
- [MeshLab Software for repairing and refining 3D files (Windows only: virtual machine or physical device needed)](https://www.meshlab.net/)

## Step 2: Setting Up Environment
On WindowsOS, open Shell Commands. On MacOS, open Terminal application. Then, copy and paste the following code to run corresponding commands in the Windows Shell or Mac Terminal window:

Install Python via Homebrew (if not installed already):
```bash
brew install python
```

Check Python version to make sure it's above 3.8:
```bash
python3 --version
```

Create and activate a Python virtual environment:
```bash
python3 -m venv ~/idc-env
source ~/idc-env/bin/activate
```

There should be `(idc-env)` infront of the terminal prompt. This indicates that a virtual Python environment is active. If not, repeat the previous steps and check for error codes.

## Step 3: Installing the Imaging Data Commons Package

Install or upgrade the IDC package by running:
```bash
pip3 install --upgrade idc-index
```

## Step 4: Downloading the Package Files

Download the sample files used in our workshop by running the command below with the desired file ID:
```bash
idc download 1.3.6.1.4.1.14519.5.2.1.4334.1501.119531128953610472040332469413
```

Upon successful completion, the terminal should prompt:
```
Successfully downloaded files to /Users/path
```

## Step 5: Moving Files to Your Working Directory

Move the downloaded files from the default download path to a preferred working directory (e.g., Desktop):
```bash
mv /Users/path/* ~/Desktop/
```

---

Congratulations! The files have been successfully downloaded and set up for editing and segmentation in DICOM-processing or STL-processing software.
