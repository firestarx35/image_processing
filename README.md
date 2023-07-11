# Group Warhall's Image Processing Programme

### This was developed as part of a team project

## Overview:
This is a command line based image processing tool developed using C++. A user can upload an image(s) and apply the following filters:

1. 2D data
 - Colour correction:
    a) Grayscale
    b) Automatic colour balance
    c) Brightness
    d) Histogram equalisation (Grayscale images)
    e) 
 - Image Blur:
    a) Median Blur
    b) Box Blur
    c) Gaussian Blur
 - Edge detection:
    a)Sobel
    b) Prewitt
    c) Scharr
    d) Robert's Cross
 2. 3D data
 - Blur:
    a)3D Gaussian
    b)3D Median
 -Projection:
    a) Maximum Intensity Projection(MIP)
    b) Minimum Intensity Projection(MinIP)
    c) Average Intensity Projection(AIP)

Details about the filters can be found in the `Report`.


Documentation : [Link](html/index.html)


LICENSE: [Link](LICENSE)


Project Report: Report - [Link](/Group%20Warshall%20-%20Advanced%20Programming%20Group%20Report.pdf)


Windows executable: [Link](main.exe)


Mac executable: [Link](main)


Tests: [Link](src/test.cpp)

# File Introduction


Images:

    Example 2D image inputs.

Images/Output:
     
    2D images:
        - Contains directories for each 2D input image.
        - Each directory contains output from each implemented filter.
    3D images:
        -Contains directories for each 3D input.
        - Four sub folders under this directory represent four methods of orthographic projections for confuciusornis and fractures CT scan datasets respectively. Each projection contains four images of without filters, with a 3d gaussian filter with kernal size of 3, with a 3d median filter with kernal size of 5, without any filters but operating on a slab.

        - slicing_x_z.png: Slice in the x-z plane with a constant y value.

        - slicing_y_z.png: Slice in the y-z plane with a constant x value.



Scans:

    Folder for downloading CT scans datasets and necessary images for testing.

html:

    Relative file for code documentation.
    Double click index.html to check the code documentation.

src:

    Source code of the project.

    - main.cpp:

        Main method for building the UI.
        
    - test.cpp:
        Functions for unit test.
        
    Each other .cpp file is a class owning an accociated .h file.

- Documentation.txt: Instructions on installing and running the project.

- Doxyfile: Configuration file for generating code documentation.

- LICENSE: The project license.

- makefile: Script for compiling and building the project.

- main: The executable tool for MAC.

- main.exe: The executable tool for windows.

- Group Warshall - Advanced Programming Group Report.pdf: Project report.

# Run the project:
- ./main in command line for mac.

- ./main.exe in command line for windows.

- build from source code:
```
    make main
    ./main
```

- input the required parameters following the prompt

# Run the test:
- build from source code:
```
    make test
    ./test
```
