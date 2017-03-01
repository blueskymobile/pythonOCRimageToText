# pythonOCRimageToText
This script convert image to text using tesserocr
tesserocr

A simple, Pillow-friendly, wrapper around the tesseract-ocr API for Optical Character Recognition (OCR).

TravisCI build status Latest version on PyPi
Supported python versions

tesserocr integrates directly with Tesseract's C++ API using Cython which allows for a simple Pythonic and easy-to-read source code. It enables real concurrent execution when used with Python's threading module by releasing the GIL while processing an image in tesseract.

tesserocr is designed to be Pillow-friendly but can also be used with image files instead.

Requirements

Requires libtesseract (>=3.04) and libleptonica (>=1.71).

On Debian/Ubuntu:

$ apt-get install tesseract-ocr libtesseract-dev libleptonica-dev
You may need to manually compile tesseract for a more recent version. Note that you may need to update your LD_LIBRARY_PATH environment variable to point to the right library versions in case you have multiple tesseract/leptonica installations.

Cython is required for building and optionally Pillow to support PIL.Image objects.

Installation

$ pip install tesserocr
