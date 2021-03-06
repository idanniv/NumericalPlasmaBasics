# Numerical Plasma Basics
## Contents
This repository includes:
 1. Integrator codes of Boris method and finite difference time domain (FDTD) method on a 1d Yee lattice.
 2. Plotting GUI to use for examples
 3. Documentation explaining the numerical methods
## Files
### Integrators
The integrator code is in C++14. This is in **QtGUI/Integrators** folder.
### QtGUI
The provided GUI is written in Qt 5.14 and uses the external library (in the repository) QCustomPlot, both under the GPL licence. The build provided is for Windows 64 bit including all the necessary DLLs. Building for other systems can be done using qt libraries. This is in **QtGUI** folder.
### Documentation
The documentation is PDF file with brief explanation of the used methods and what can be learned applying them. The file contains relevant references for further explanation. The file is under **Documentation** folder.
## Future improvements
The C++ could use expression templates or std::ranges for delayed evaluation. This would prevent the memory allocation of intermediate temporaries and provide a significant speed improvement.

Make a C++ extension to a python module and benchmark improvements.

The GUI could be more stable by running the computation on a different thread. Running the GUI with extreme parameter values could cause a crash.

When GUI saving the figure also print the parameters used.

GUI implement a play button for continously integrating and displaying animation.
