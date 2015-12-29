Virtual Scrapbook is a multi-touch based image and video viewer.Users can move,zoom and rotate multiple images/videos simultaneously using multi-touch gestures.Touches are made when an Infra Red pen is moved on an acrylic glass slab.
Detection is done using OpenCV

Installation

---


The Virtual Scrapbook contains both the software and the hardware implementation.

Hardware

---


An acrylic board is placed on a metal frame and acts as the table.The InfraRed pen is dragged across the acrylic board
and this helps to register the touches.The camera captures the co-ordinates from underneath the acrylic board using
OpenCV and sends them to PyMT using TUIO protocol.

Software

---


Front-End - PyMT (python library)
Detection - OpenCV (C++)
Calibration - Octave API for C++ (C++) with GUI created using Qt4
Communication - TUIO (C++)

PyMT can be downloaded from http://pymt.eu/wiki/DevGuide/GrabSourceCode
> python setup.py install

OpenCV can be downloaded from http://opencv.willowgarage.com/wiki/

Octave API for C++ is available at http://octave.sourceforge.net/doxygen/html/

TUIO can be found at http://www.tuio.org/?software
The link to the C++ API is as follows
http://sourceforge.net/projects/reactivision/files/TUIO%201.0/TUIO-Clients%201.4/TUIO_CPP-1.4.zip/download

Refer README for more details