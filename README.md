# Training an Object Detection Model with TensorFlow OCR Invoice Extractor

## How to Run

To use your images instead of the provided ones:
1. Fork and clone this repository to your local machine.
   ```
   git@github.com:hrushikesh009/TensorFlow-OCR-Invoice-Extractor.git
   ```

2. Install required libraries.
   ```
   pip3 install -r requirements.txt
   ```

3. **Step 1: Annotate Images**
   - Save photos with your objects to `./data/raw`.
   - Resize images to `(800, 600)` with:
     ```
     python resize_images.py --raw-dir ./data/raw --save-dir ./data/images --ext jpg --target-size "(800, 600)"
     ```
   - Train/test split into `./data/images/train` and `./data/images/test`.
   - Annotate resized images with [labelImg](https://tzutalin.github.io/labelImg/) and generate `xml` files.

4. **Step 2: Open Colab Notebook**
   - Open the Python Notebook (Tensorflow-object-detection-training), which includes a comprehensive guide with a markdown on each stage of building a Tensorflow OCR model.

Enjoy the journey!