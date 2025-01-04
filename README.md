Polygon Detection using OpenCV

Overview
This project provides a Python script that detects polygons in an image using OpenCV. The script outputs a text file containing the name and coordinates of the centroid of each detected polygon, as well as an image showing the centroid of each polygon.

Requirements
- OpenCV 4.x or later
- Python 3.x or later
- NumPy

Usage
1. Clone the repository or download the script.
2. Install the required dependencies using pip: `pip install opencv-python numpy`
3. Run the script using Python: `python (link unavailable) -i input_image.jpg -o output.txt -c output_image.jpg`

Command-Line Arguments
- `-i` or `--input`: Input image file path.
- `-o` or `--output`: Output text file path.
- `-c` or `--centroid_image`: Output image file path showing centroids.

Example Usage
- Detect polygons in an image and output the results to a text file and an image: `python (link unavailable) -i input_image.jpg -o output.txt -c output_image.jpg`

Code Explanation
The script uses the following steps to detect polygons in an image:

1. Load the input image using OpenCV.
2. Convert the image to grayscale and apply thresholding to segment out the polygons.
3. Find the contours of the polygons using OpenCV's `findContours` function.
4. Iterate through the contours and use OpenCV's `approxPolyDP` function to approximate the polygon shape.
5. Calculate the centroid of each polygon using OpenCV's `moments` function.
6. Write the name and coordinates of the centroid of each polygon to the output text file.
7. Draw the centroid of each polygon on the output image.

Output
The script outputs two files:

- `output.txt`: A text file containing the name and coordinates of the centroid of each detected polygon.
- `output_image.jpg`: An image showing the centroid of each detected polygon.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgments
This project uses OpenCV, a computer vision library developed by Intel. See the OpenCV website for more information.
