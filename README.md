
# Py2DSpectroscopy
This is a fork of https://github.com/SvenBo90/Py2DSpectroscopy

Py2DSpectroscopy is a light weight Python UI code for the analysis of two-dimensional spectroscopy data. It was designed to analyze photoluminescence maps of two-dimensional materials such as MoS_2. 

## Video Tutorial

A video tutorial is available on Youtube.

[![Video Tutorial](http://img.youtube.com/vi/NfRWFomUZM0/0.jpg)](http://www.youtube.com/watch?v=NfRWFomUZM0 "Py2DSpectroscopy Video Tutorial ")

## Requirements

* Python 3.5
* PyQt5 
* Matplotlib 2.0.0
* NumPy 1.12.0
* SciPy 0.18.0
* Skimage 0.12.3
* cmcrameri 1.9

## Features

* load and browse two-dimensional spectroscopy data
* remove background from the data
* remove cosmic rays from the data
* align microscope images (e.g. AFM or SEM) with the data
* fit the data

## Supported Data Formats

Currently, two data formats are supported. 

The first data format is a simple .txt file. The first line of the file gives the energies and all further lines give the counts for each pixel, whereas the first and second column of each line give the x and y positions. An example map can be downloaded: https://drive.google.com/open?id=0B-hxzhGGvvMSVVdYRGN1NVZlNVU.

Below an example table is provided for reference.

| X  | Y  | E0    | E1    | EN    |
|----|----|-------|-------|-------|
| X0 | Y0 | S00_1 | S00_2 | S00_N |
| X0 | Y1 | S01_1 | S01_2 | S01_N |
| X0 | YN | S0N_1 | S0N_2 | S0N_N |
| X1 | Y0 | S10_1 | S10_2 | S10_N |
| X1 | YN | S1N_1 | S1N_2 | S1N_N |
| XN | YN | SNN_1 | SNN_2 | SNN_N |

The second data format is a .dat file, that comes along with .asc spectra files. The .dat includes a table, where the first, second and third column are the pixel number, the x pixel position and the y pixel position, respectively. Further columns can give information on temperature, excitation power or similar quantities measured during the scanning. The spectra file have the format spectrum_X_Y.asc and include a column for the wavelength and a column for the counts. An example map can be downloaded: https://drive.google.com/open?id=0B-hxzhGGvvMSUHJ6SWg3NndUVEE

# Screenshots
![Screenshot 1](https://preview.ibb.co/nHnJqk/screen1.png "Screenshot 1")
![Screenshot 2](https://preview.ibb.co/jYH7i5/screen2.png "Screenshot 2")
