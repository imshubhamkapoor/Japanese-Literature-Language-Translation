# Japanese-Literature-Language-Translation

In this project, there is a dataset of Kanji VG characters. Kanji is used as the modern japanese language that consist of Sinographs. For each character, it provides a SVG file that gives the shape, direction and of each of its strokes. There is a second folder of Kanji VG that consist of the pixel format which are converted from these SVG files. Using KanjiVG, it is very easy to create stroke order diagrams or animations, kanji dictionaries, and many more. 

The project until now consist of following steps:
* Loading the SVG and converting into PNG file format.
* Loading the PNG dataset and preprocessing.
* Building and training a Convolutional Variational Autoencoder on the dataset.
* Building and training a Convolutional Variational Autoencoder on the dataset.
* Using the decoder to generate sample Kanji VG characters.

The whole project is implemented using pytorch in jupyter notebook.

## Files Description

- **KanjiVG-SVG** It consist of a single zipped folder with 11456 files of Kanji VG in SVG format. The vector size is 64 by 64.
- **KanjiVG-Pixel** It consist of a single zipped folder with 11456 files of Kanji VG in PNG format converted from KanjiVG-SVG. The image size is 28 by 28 pixels.
- **SVG2PNG.ipynb** It is used to load and convert the images from SVG to PNG
- **CNN-VAE.ipynb** It is used to build the CNN-VAE model using the jupyter notebook. It can be used independently to see how the model works.
- **VAE.ipynb** It is used to build the VAE model using the jupyter notebook. It can be used independently to see how the model works.

## Installation

The Code is written in Python 3.6.5 . If you don't have Python installed you can find it here. If you are using a lower version of Python you can upgrade using the pip package, ensuring you have the latest version of pip.

Additional Packages that are required are: Numpy, Svglib, Pytorch, PIL. You can donwload them using pip.
