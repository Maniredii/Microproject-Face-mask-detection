# Microproject – Face Mask Detection

A lightweight, real-time face mask detection system using deep learning models—ideal for monitoring and enforcing mask compliance in video streams and static images.

## Features

* **Image & Video Detection**: Detects masks in both static images and live video feeds.
* **Multiple Model Support**: Includes pre-trained models like ResNet50\_v2 and InceptionV3 for better accuracy.
* **Web Interface**: `app.py` enables seamless deployment via a simple web application.
* **Model Conversion**: `model2onnx.py` facilitates converting trained models into ONNX format for broader compatibility.
* **Training Pipeline**: `train_mask_detector.py` allows retraining and fine-tuning of the model.
* **Visual Analytics**: Includes `plot.png` to show model performance trends over epochs.
* **Cross-Platform Guidance**: Comprehensive setup instructions with Windows reference in `Windows_guide.md`.
* **Documentation & Presentation**: Includes a project report (`MANIDEEP REDDY MICRO PROJECT REPORT .pdf`) and presentation slides.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Maniredii/Microproject-Face-mask-detection.git
   cd Microproject-Face-mask-detection
   ```
2. Install required Python packages:

   ```bash
   pip install -r requirements.txt
   ```

## Usage

* **Static Image Detection**:

  ```bash
  python detect_mask_image.py --image path/to/image.jpg
  ```

* **Live Video Detection**:

  ```bash
  python detect_mask_video.py
  ```

* **Run Web Application**:

  ```bash
  python app.py
  ```

  Navigate to `http://localhost:5000` to interact with the detection tool via your browser.

* **Convert Model to ONNX Format**:

  ```bash
  python model2onnx.py --model mask_detector.model --output mask_detector.onnx
  ```

* **Train a New Model**:

  ```bash
  python train_mask_detector.py
  ```

## Directory Overview

| Path                                   | Description                                     |
| -------------------------------------- | ----------------------------------------------- |
| `ResNet50_v2/`, `incep_v3_mask_model/` | Model directories containing architectures.     |
| `face_detector/`                       | Face detection utilities and scripts.           |
| `images/`, `Readme_images/`            | Sample images and documentation visuals.        |
| `search.py`                            | Utility for dataset searching or preprocessing. |
| `.pptx`, `.pdf`, `.md` files           | Presentation, report, and guides.               |

## Contributions

Contributions are welcome! Feel free to open issues or submit pull requests for:

* New features or mask detection configurations
* Enhancements to UI or UX
* Additional platform support or framework conversion

## License

Licensed under the **MIT** License — see the [LICENSE](LICENSE) file for details.
