# Protective-Equipment-detector

This project leverages a **custom-trained YOLOv8 model** to detect protective equipment (e.g., helmets, vests) in both **images** and **videos**. It includes a user-friendly **Gradio interface** for uploading files and viewing annotated outputs, along with missing equipment summaries.

---

## Features

- **Image Detection**: Detect protective equipment in images and display missing items along with annotated results.
- **Video Detection**: Process videos to detect missing equipment frame-by-frame and generate annotated output videos.
- **Custom YOLOv8 Model**: Utilizes a YOLOv8 model trained on customized datasets for high-accuracy detection.
- **Gradio Interface**: Easy-to-use interface for uploading files and viewing results.

---

## Getting Started

### Prerequisites

1. Python 3.8 or later
2. Install required Python packages:
   ```bash
   pip install gradio ultralytics opencv-python-headless
   ```
---

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/KHADIJAELHAOU/Protective-Equipment-detector.git
   cd Protective-Equipment-detector
   ```
   Here's the updated README file reflecting that users simply need to run all cells in the Colab notebook to install libraries, load the model, and test the program:

---



## Usage in Google Colab

### Steps to Run the Project
1. Open the provided Colab notebook file (`Protective-Equipment-Detector.ipynb`) in Google Colab.
   - Either download the notebook from the repository and upload it to Colab or directly open the notebook via its public link.

2. **Run All Cells**:
   - This will:
     - Install all required libraries.
     - Load the custom-trained YOLOv8 model (`best.pt`).
     - Launch the Gradio interface for image and video detection.

3. **Interact with the Gradio Interface**:
   - Once the interface launches, a public URL will be generated by Gradio.
   - Open the URL in your browser.
   - Upload an image or video file for detection.

4. **Output**:
   - **Images**: Annotated images with missing equipment highlighted will be saved to `/content/annotated_image.jpg`.
   - **Videos**: Annotated videos will be saved to `/content/annotated_video.mp4`.

---



---

## Example Usage

### Image Detection
1. Open the Colab notebook.
2. Upload an example image to the Gradio interface and then submit.
3. View the annotated image (saved to `/content/annotated_image.jpg`) in the interface.

### Video Detection
1. Open the Colab notebook.
2. Upload an example video to the Gradio interface and then submit.
3. View the annotated video (saved to `/content/annotated_video.mp4`) in the interface .

---

## Technical Details

### YOLOv8 Custom Model
- **Classes**:
  - `helmet`
  - `vest`
- The YOLOv8 model was trained using the [Ultralytics YOLOv8 framework](https://github.com/ultralytics/ultralytics) on a custom dataset from roboflow.

### Gradio Interface
- **Supported Input Types**:
  - Image files: `.jpg`, `.png`
  - Video files: `.mp4`

---

## Requirements

No manual installation is needed. Running all cells in the Colab notebook will:
- Install required Python libraries (`gradio`, `ultralytics`, `opencv-python-headless`).
- Load the YOLOv8 model.
- Launch the Gradio interface.

---
