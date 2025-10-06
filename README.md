# Traffic Sign Detection With YOLO8

## Project Description
This project implements a robust computer vision system for traffic sign detection using the YOLOv8 object detection framework. The core innovation is the inclusion of a spoofed stop sign filtering mechanism designed to distinguish legitimate Stop Signs from potentially malicious or erroneous detections.

---

## Key Features
* **Real-time Object Detection:** Uses the **YOLOv8 (Ultralytics)** model for high-performance detection of traffic signs (specifically Stop Signs and Persons).
* **Spoof Detection:** Implements custom logic to filter out detected objects that do not meet criteria for a real "Stop Sign," labeling them as "Spoofed Stop".
* **Visualization:** Leverages **OpenCV** (`cv2`) to draw bounding boxes and labels, using distinct colors to clearly distinguish between standard detections, person detections, and spoofed stop signs.
* **Data Integration:** Utilizes the **Kaggle API** (`kagglehub`) to access and manage the required dataset for training and testing.

---

## Installation and Usage
1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/sarahelfeel04/Traffic-Sign-Detection-With-YOLO8.git](https://github.com/sarahelfeel04/Traffic-Sign-Detection-With-YOLO8.git)
    cd Traffic-Sign-Detection-With-YOLO8
    ```
2.  **Data Setup:**
    * The project uses the `pkdarabi/cardetection` dataset from Kaggle. You'll need to set up your Kaggle API key to download the data to the expected path (e.g., `/kaggle/input/cardetection/car/train/images`).
    ```python
    import kagglehub
    kagglehub.dataset_download('pkdarabi/cardetection') 
    ```
3.  **Run the project:**
    Run the jupyter notebook after all necessary libraries are installed.
