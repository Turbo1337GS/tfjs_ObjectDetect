# Object Detection

This is the code for a simple web application that performs object detection using TensorFlow.js and the COCO-SSD model. The application allows the user to select an image file and then detects objects within the image, displaying their names and confidence scores.

 * https://main.gigasoft.com.pl/Object%20Detect/index.html


## Usage

To use this application, follow these steps:

1. Clone the repository or download the HTML file.
2. Open the HTML file in a web browser.
3. Click the "Choose File" button to select an image from your local machine.
4. The image thumbnail will be displayed, and the "Detect" button will appear.
5. Click the "Detect" button to start the object detection process.
6. After the detection is complete, the detected objects will be listed along with their confidence scores.
7. Additionally, three columns with different colors will be displayed to represent the confidence scores in a visual way.

## Dependencies

This application relies on the following dependencies:

- TensorFlow.js v3.3.0
- COCO-SSD model

These dependencies are loaded from CDN links provided in the HTML file.

## How It Works

1. The user selects an image file using the "Choose File" button.
2. The selected image is displayed as a thumbnail.
3. After the user clicks the "Detect" button, the `detectObjects()` function is triggered.
4. In the `detectObjects()` function, the necessary DOM elements are accessed and initialized.
5. The COCO-SSD model is loaded asynchronously using `cocoSsd.load()`.
6. Once the model is loaded, the `model.detect()` function is called to perform object detection on the selected image.
7. The detected objects along with their confidence scores are collected and displayed.
8. The height of the three columns representing the confidence scores is adjusted based on the scores.
9. Finally, the UI elements are updated to reflect the detection results.

Feel free to modify and customize this code to fit your needs. Happy object detection!
