🐘 Elephant Detection Using OpenCV

This project demonstrates a simple yet effective method to detect elephants in an image using OpenCV and basic color thresholding techniques. It also includes an interactive image display that allows users to click on an image and view the RGB values at specific points.

📌 Features

* Loads and displays an image of an elephant.
* Allows users to interactively click on the image and retrieve RGB values.
* Samples specific pixel coordinates and displays their RGB values.
* Marks selected points on the image for reference.
* Applies simple RGB color thresholding to detect elephant regions.
* Visualizes the final detected region in grayscale.

 🧰 Technologies Used

* Python 3
* OpenCV
* NumPy
* Matplotlib
* IPyWidgets
* IPyEvents
* PIL (Pillow)
* Google Colab (for execution)

🔍 How It Works

1. The image is loaded and converted to RGB.
2. Several sample coordinates are selected, and the RGB values of these pixels are printed.
3. The selected points are marked on the image using colored circles and labels.
4. A basic RGB thresholding technique is used to segment the elephant from the background.
5. The binary mask (black and white image) shows the region where the elephant is detected.

 🎯 Sample Thresholding Logic

```python
if(lower_thresh[0] <= r <= upper_thresh[0] and
   lower_thresh[1] <= g <= upper_thresh[1] and
   lower_thresh[2] <= b <= upper_thresh[2]):
    elephant_detected[x, y] = 0
else:
    elephant_detected[x, y] = 255
```

🖱️ Interactive Demo

* Click on any part of the image to retrieve the RGB values at that point.
* This is useful for calibrating or adjusting your detection thresholds.

📷 Example Output

* Original image with marked points
* Console output of clicked RGB values
* Final grayscale image highlighting the detected elephant

 📂 How to Run

1. Clone the repository.
2. Open the notebook `Elephant Detection.ipynb` in Google Colab or Jupyter Notebook.
3. Upload an image named `elephant.jpg` or change the path accordingly.
4. Run the notebook cells sequentially.

 ✅ Requirements

Install the required packages (if running locally):

```bash
pip install opencv-python matplotlib numpy ipywidgets ipyevents pillow
```

> 📝 This notebook is best run on Google Colab for full interactivity.

💡 Future Enhancements

* Use contour detection to draw boundaries around the elephant.
* Train a machine learning model for more robust detection.
* Replace manual RGB thresholding with HSV or Lab color space segmentation.


