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

3. **Custom YOLOv8 Model**: Place your trained YOLOv8 model file (e.g., `best.pt`) in the appropriate directory.

---

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/KHADIJAELHAOU/Protective-Equipment-detector.git
   cd Protective-Equipment-detector
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

---

## Usage

1. **Run the Application**:
   ```bash
   python app.py
   ```

2. **Interface Overview**:
   - Upload an image or video using the Gradio interface.
   - Select the input type (`Image` or `Video`).
   - Submit

3. **Output**:
   - **Images**: The annotated image will highlight detected equipment and indicate missing items.
   - **Videos**: The annotated video will include frame-by-frame detection .

---



## Example

### Image Detection
1. Upload an image (e.g., workers wearing safety gear).
2. Output: Annotated image with missing equipment identified.

![example_image](example_inputs/example_output.jpg)

### Video Detection
1. Upload a video (e.g., surveillance footage).
2. Output: Annotated video highlighting missing equipment frame-by-frame.

---

## Technical Details

### YOLOv8 Custom Model
- The YOLOv8 model was trained on a custom dataset with classes:
  - `helmet`
  - `vest`
  
- Training was performed using the [Ultralytics YOLOv8 framework](https://github.com/ultralytics/ultralytics).

### Gradio Interface
- Designed for ease of use.
- Supports:
  - Image files: `.jpg`, `.png`
  - Video files: `.mp4`, `.avi`

---

## Requirements

- **Python 3.8+**
- **Dependencies**:
  - `gradio`
  - `ultralytics`
  - `opencv-python-headless`

Install all dependencies using:
```bash
pip install -r requirements.txt
```

---
