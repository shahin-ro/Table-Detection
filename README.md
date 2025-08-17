# Table-Detection
Table Extraction and OCR for Persian Documents 📄✨
This project provides a Python-based solution for detecting table structures in images and extracting Persian text using Optical Character Recognition (OCR). It uses OpenCV for table detection and Tesseract OCR for text extraction, with proper rendering of Persian text. 🚀
Features 🌟

Table Detection 📊: Identifies table cells in images using advanced image processing with OpenCV.
OCR Support 🔍: Extracts Persian text from table cells using Tesseract OCR with Persian language support.
Data Structuring 📈: Organizes extracted text into a Pandas DataFrame for easy analysis.
Visualization 🎨: Displays detected table cells, line masks, and intersection points for verification.

Requirements 🛠️
To run this project, you need the following dependencies:

Python 3.7+ 🐍
OpenCV (cv2)
NumPy
Matplotlib
Pandas
Pytesseract (for Tesseract OCR)
Tesseract-OCR with Persian language support (tesseract-ocr-fas)

Install the dependencies using:
pip install opencv-python numpy matplotlib pandas pytesseract

For Tesseract OCR:
apt-get install -y tesseract-ocr tesseract-ocr-fas

Usage 🚀

Clone the Repository 📂:
git clone https://github.com/your-username/table-extraction-ocr.git
cd table-extraction-ocr


Prepare an Image 🖼️:

Ensure you have an image containing a table with Persian text (e.g., a scanned document or screenshot).
Place the image in the project directory or provide the path to the script.


Run the Script ▶️:

The script (jadval.py) processes the image, detects table cells, extracts text, and visualizes the results.
Run the script:python jadval.py



Output 📜:

The script outputs:
A count of detected table cells ✅.
Extracted text for each cell with coordinates 📍.
A Pandas DataFrame representing the table structure 🗃️.
Visualizations showing detected cells, line masks, and intersection points 🖼️.



How It Works 🧠

Table Detection 📏:

Uses OpenCV to preprocess the image (grayscale, adaptive thresholding, morphological operations).
Detects horizontal and vertical lines to identify table boundaries.
Clusters line intersections to determine cell coordinates.


Text Extraction 📝:

Crops each detected cell and processes it with Tesseract OCR (lang='fas') for Persian text extraction.
Stores text and coordinates for each cell.


Data Structuring 📚:

Maps extracted text to a grid based on cell positions.
Creates a Pandas DataFrame to represent the table structure.


Visualization 🖌️:

Displays three plots:
Detected Cells 🟢: Original image with green rectangles around table cells.
Line Mask ⚪: Inverted mask showing detected horizontal and vertical lines.
Joints 🔲: Intersection points of table lines.


Notes 📌

Tesseract OCR 🔍: Requires tesseract-ocr-fas for Persian language support.
Colab Compatibility ☁️: The script is designed to work in Google Colab, with file upload support and Tesseract installation commands.
Image Quality 🖼️: OCR accuracy depends on clear table lines and readable text.

Limitations ⚠️

The table detection algorithm assumes well-defined table lines.
OCR accuracy depends on image quality and text clarity.
Persian text rendering in visualizations may require additional font support for non-Colab environments.

Contributing 🤝
Contributions are welcome! Please submit a pull request or open an issue for bug reports, feature requests, or improvements. 🙌
License 📜
This project is licensed under the MIT License. See the LICENSE file for details.
Acknowledgments 💖

OpenCV for image processing 🖼️.
Tesseract OCR for Persian text extraction 🔍.
Pandas for data structuring 📚.

