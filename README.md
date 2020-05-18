# Binary-Image-Segmentation

Binary Image segmentation is the process of classifying the pixels of an image into two categories: pixels belonging to the foreground objects of an image and pixels belonging to the background objects of an image.

In this project, we were asked to  implement a simple binary image segmentation technique using min-cut and the OpenCV library.

The binary image segmentation problem can be reduced to finding a minimum cut in the graph induced by the image graph: the pixels are the vertices or nodes in the graph and we have edges between any neighboring pixels in the horizontal and vertical direction (i.e. any vertex has maximum 4 neighbours).

The program has 3 arguments: an input image, a configuration file that provides the initial set of foreground and background points and an output image. Your program has to compute the binary segmentation of the pixels in the input image based on the initial segmentation provided in the configuration file. The output has to be an image
of the same size of the input image such that each pixel is either white (foreground) or black (background).

Example: ./seg simple.png config.txt result.png
