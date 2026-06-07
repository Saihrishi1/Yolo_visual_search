# YOLO Image Search System
## ABSTRACT
The YOLO Image Search System is a computer vision application developed using YOLOv11 for object detection and image retrieval. The system detects objects present in images, generates metadata from detection outputs, and allows users to search images using object-based filters. An interactive Streamlit interface is used to process images, visualize results, and perform intelligent image searches.

## Dataset & YOLO Model Details (COCO)
This project uses the COCO dataset classes, which contain 80 common object categories such as person, car, dog, cat, airplane, and banana. The detection model used is YOLOv11, chosen for its fast inference speed, improved accuracy, and real-time object detection capability. The model predicts object classes, bounding boxes, and confidence scores which are later converted into searchable metadata.

## Environment Setup
Before running the project, install:

### Prerequisites
Python 3.11

Anaconda / Miniconda

Visual Studio Code (VS Code)

NVIDIA GPU (Optional – for GPU acceleration)

### Open the project folder inside VS Code.

Required project files:

```
requirements.txt
instructions.txt
app.py
```

### Open terminal in VS Code:

```
View → Terminal
```
### GPU Installation Steps

Step 1 – Create Conda Environment
```
conda create -n yolo-image-search-gpu python=3.11 -y
```

Step 2 – Activate Environment
```
conda activate yolo-image-search-gpu
```

Step 3 – Install PyTorch with CUDA Support
```
conda install pytorch torchvision pytorch-cuda=12.4 -c pytorch -c nvidia
```

Step 4 – Install Project Dependencies
```
pip install -r requirements.txt
```

### How to Run in VS Code using Conda

Activate Environment
```
conda activate yolo-image-search-gpu
```

Launch the Streamlit interface
```
streamlit run app.py
```

The terminal will display and Open Browser:
```
Local URL: http://localhost:8501
```

### Features Available in UI:

Upload image dataset

Select YOLOv11 model

Process images

Generate metadata

Apply search filters

Display results grid

Export JSON output

## Output:

<img width="1901" height="900" alt="597966268-c4f57d76-3979-4eee-9c10-a34fc93790a3" src="https://github.com/user-attachments/assets/e82d6d7e-7353-4f00-b26b-d82463ab76ec" />

<img width="1920" height="1020" alt="597966536-3c065d2e-25a3-426d-b8b4-e13fc8d91e7f" src="https://github.com/user-attachments/assets/77181cd5-12bb-437a-b0c3-d3c5968a3b24" />

<img width="1920" height="1020" alt="597966615-1d6821b2-8fe2-4948-baa2-08d7534113bf" src="https://github.com/user-attachments/assets/2aae7e7e-924a-498b-bb60-3e6e0a3e8c73" />

<img width="1920" height="1020" alt="597966695-3167e7fe-2333-44b0-a3a5-36fea7890409" src="https://github.com/user-attachments/assets/3661e01a-a366-41cb-949a-eb387f949394" />

<img width="1919" height="1022" alt="597966887-78747f74-d24d-485d-9300-7467c83da542" src="https://github.com/user-attachments/assets/90533d43-4a3c-40b7-96d4-392dafd7f0e9" />

<img width="1919" height="1017" alt="597966991-176a74fa-7299-4970-a57b-b28ecc294d31" src="https://github.com/user-attachments/assets/ff566598-56b7-4f15-8d61-189ddcc2d3d4" />

## Enhancements
The system goes beyond basic object detection by introducing metadata-based image searching. Detection outputs are stored in JSON format, allowing fast querying without rerunning inference. The application also supports logical filtering using AND/OR conditions, threshold-based searches, and loading previously generated metadata for quicker execution. The modular pipeline improves scalability and maintainability.

## Result & Conclusion
The YOLO Image Search System successfully performs object detection, metadata generation, and image retrieval using YOLOv11. The Streamlit interface provides a simple and interactive user experience, while reusable metadata reduces repeated computation. Overall, the project demonstrates an effective combination of computer vision, metadata engineering, and UI deployment for building an intelligent image search system.





