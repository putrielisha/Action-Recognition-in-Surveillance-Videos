# Action-Recognition-in-Surveillance-Videos
A deep learning-based surveillance analysis system that integrates Faster R-CNN and SlowFast architectures to perform real-time object detection and action classification on CCTV video streams. The pipeline generates bounding boxes around detected individuals and assigns action labels with confidence scores to support automated video monitoring.

# System Pipeline
Video Input → Faster R-CNN → Bounding Boxes → SlowFast Model → Action Classification → Annotated Output

# Technologies Used
- Python
- PyTorch
- MMDetection
- Faster R-CNN
- SlowFast
- OpenCV

# Features
- Object detection of individuals in CCTV footage
- Action recognition using deep learning models
- Bounding box visualization
- Confidence scoring for predictions
- Annotated video output generation

# Demo
[Video Demo](https://youtu.be/vqq9JxCmGQY)

This demo showcases the system’s full surveillance pipeline in operation. A video input is processed frame-by-frame, where individuals are first detected using Faster R-CNN and enclosed within bounding boxes. Each detected person is then assigned action labels along with confidence scores using the SlowFast action recognition model.

A rule-based decision layer is applied on top of the model outputs to flag predefined behaviors such as “carry” and “hold” as “Suspicious”. This indicator is displayed directly on the output frame to demonstrate real-time event interpretation.

The demo highlights the integration of object detection, temporal action recognition, and rule-based classification within a single surveillance analysis pipeline.

# Limitations
- Performance affected by camera angle and lighting conditions
- Limited robustness in crowded or occluded scenes
- Requires high computational resources for real-time processing

# Future Improvements
- Pre-incident behavior detection (e.g., loitering, crowd anomalies)
- Sequence-based action analysis
- Timestamped event logging for easier review
- GPU optimization for real-time deployment

# Report
Full technical report included in this repository.
