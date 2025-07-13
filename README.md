# Image-Contour-Detection-using-OpenCV

This project demonstrates a basic image processing pipeline using OpenCV in Python. It loads an image, converts it to grayscale, applies Gaussian blur, detects edges using the Canny algorithm, finds contours, and draws those contours on the original image. The code is implemented in a Jupyter notebook (OpenCv.ipynb) and uses OpenCV, NumPy, and Matplotlib libraries.

Usage

Using Google Colab (Recommended)





Open Google Colab.



Upload the OpenCv.ipynb notebook by clicking File > Upload Notebook.



Run the first cell to import the required libraries (cv2, numpy, matplotlib).



When prompted by the files.upload() function, upload an image file from your local machine.



Run the remaining cells in order to process the image and display the original and contoured images.

Running Locally





Ensure you have Python installed along with the following libraries:





OpenCV (cv2)



NumPy



Matplotlib



Install the dependencies using pip:
```
pip install opencv-python numpy matplotlib
```


Open the OpenCv.ipynb notebook in Jupyter Notebook or JupyterLab.



Replace the file upload code with a local image path:
```
img_path = 'path/to/your/image.jpg'  # Replace with your image path
```
For example, remove or comment out:
```
from google.colab import files
uploaded = files.upload()
img_path = next(iter(uploaded.keys()))
```
And use:
```
img_path = 'path/to/your/image.jpg'

```

Run the cells in order to process the image and display the results.

Note: Ensure all cells are executed sequentially, as later cells depend on functions defined earlier.

Notebook Sections





Import Libraries: Imports OpenCV, NumPy, and Matplotlib.



Define Utility Functions: Includes functions for loading (load_image) and displaying (display_image) images.



Preprocessing & Edge Detection: Converts the image to grayscale (to_grayscale), applies Gaussian blur (gaussian_blur), and detects edges (detect_edges) using Canny.



Contour Finding & Drawing: Finds contours (find_contours) and draws them on the image (draw_contours).



Process Image: Uploads an image (in Colab) or loads from a path (locally), processes it, and displays the results.

Customization




```
Edge Detection Parameters: Adjust low and high thresholds in detect_edges (e.g., detect_edges(img_gray, low=50, high=150)) for better edge detection.



Blur Kernel Size: Modify ksize in gaussian_blur (e.g., gaussian_blur(img, ksize=7)), ensuring it’s an odd number.



Contour Appearance: Change color (e.g., (0, 255, 0) for green) and thickness (e.g., 2) in draw_contours.
```

Contributing

Feel free to fork the repository and submit pull requests for improvements or bug fixes.

