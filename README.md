# Vision Transformers for Object Detection and Depth Estimation

A computer vision project that combines two state-of-the-art **Hugging Face Transformers** models to perform **Object Detection** and **Monocular Depth Estimation** from a single input image.

The project demonstrates how multiple pre-trained vision models can be integrated into a unified image analysis pipeline.

---

## Features

* Object Detection using DETR
* Monocular Depth Estimation using DPT
* End-to-end image processing pipeline
* Automatic visualization of predictions
* Overlay generation combining detections and depth maps
* GPU acceleration with PyTorch

---

## Models Used

### DETR (Detection Transformer)

**Model**

```text
facebook/detr-resnet-50
```

Used for:

* Object detection
* Bounding box prediction
* Object classification

---

### DPT (Dense Prediction Transformer)

**Model**

```text
intel/dpt-large
```

Used for:

* Monocular depth estimation
* Dense scene understanding
* Colorized depth visualization

---

## Processing Pipeline

```text
Input Image
      │
      ├────────► DETR
      │            │
      │            ▼
      │    Object Detection
      │
      └────────► DPT
                   │
                   ▼
          Depth Estimation
                   │
                   ▼
          Visualization & Overlay
```

---

## Output

The notebook generates three outputs:

* Object Detection image
* Colorized Depth Map
* Combined Overlay visualization

---

## Technologies Used

* Python
* PyTorch
* Hugging Face Transformers
* OpenCV
* NumPy
* Matplotlib

---

## Applications

* Autonomous driving
* Robotics
* Scene understanding
* Smart surveillance
* Augmented Reality
* Image analysis

