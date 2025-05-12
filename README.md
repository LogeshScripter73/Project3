
# Number Plate Detection using OpenCV and EasyOCR

This project demonstrates a simple approach to detect vehicle number plates using OpenCV and read the text using EasyOCR.

## 📌 Features

- Detects number plates using OpenCV Haar Cascades.
- Extracts and reads number plate text using EasyOCR.
- Displays the image with bounding boxes and detected plate text.

## 🖼️ Example Output

![Example Output](example_output.png) <!-- Replace with actual screenshot if available -->

## 🛠️ Requirements

Install the required Python libraries using pip:

```bash
pip install opencv-python easyocr
```

If using Google Colab, the display function should work directly using `cv2_imshow`.

## 🧠 How It Works

1. The image is read and converted to grayscale.
2. Haar Cascade classifier (`haarcascade_russian_plate_number.xml`) detects number plates.
3. Detected plates are cropped and passed to EasyOCR.
4. Detected text is drawn on the original image and displayed.

## 🚀 How to Use

1. Clone the repository or download the code.
2. Make sure the image file (e.g., `NUMPLATE.jpeg`) is in the same directory or update the path in the script.
3. Run the script:

```python
image_path = 'NUMPLATE.jpeg'
detect_number_plate(image_path)
```

If you're running locally, replace `cv2_imshow` with `cv2.imshow` and make sure GUI support is enabled.

## 📂 File Structure

```
├── detect_number_plate.py   # Python script for number plate detection
├── NUMPLATE.jpeg            # Sample image (replace with your own)
└── README.md                # Project documentation
```

## 🔍 Dependencies

- OpenCV
- EasyOCR
- NumPy
- Google Colab (for cv2_imshow, or replace for local use)

## ⚠️ Notes

- Detection accuracy may vary depending on lighting, angle, and plate clarity.
- The default Haar cascade used is for Russian-style plates and may need tuning for others.

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
