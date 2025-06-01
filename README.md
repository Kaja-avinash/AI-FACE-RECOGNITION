# AI-FACE-RECOGNITION


This project implements a simple face recognition system using OpenCV’s Haar Cascades and FisherFace recognizer. It allows you to:

- **Collect face data** via webcam and save images to a dataset.
- **Train a face recognizer** on the collected images.
- **Recognize faces live** from webcam video feed inside a Jupyter Notebook (e.g., VS Code).

---

## Features

- Real-time face detection using Haar Cascade classifier.
- Face data collection and dataset creation with a user-defined name.
- FisherFace recognizer model training and live recognition.
- Compatible with Jupyter Notebook environments, showing video frames inline.
- Keyboard interrupt support for stopping data collection or recognition.

---

## Requirements

- Python 3.x
- OpenCV (`opencv-python` and `opencv-contrib-python`)
- NumPy
- Pillow
- Jupyter Notebook or VS Code with Jupyter extension

> **Note:** The `haarcascade_frontalface_default.xml` file is included in this repository under the `models/` folder.  
> Make sure to update the `haar_file` path in the code accordingly, for example:  
> `haar_file = r'models/haarcascade_frontalface_default.xml'`

---

## Installation

1. Install required Python packages:
pip install opencv-python opencv-contrib-python numpy pillow
2.Clone or download this repository to your local machine.

3.Update the paths in the code for:

- haar_file — path to models/haarcascade_frontalface_default.xml

- datasets — folder where face data images will be saved (you can leave as default or change as needed)
# Usage
Run the notebook and execute the cell with the main code. You will see a menu:

markdown
Copy
Edit
========== Face Recognition System ==========
1. Collect Face Data
2. Recognize Faces
Enter choice (1/2):
### Option 1 (Collect Face Data):

- Enter your name.

- The webcam will open and collect 100 face images.

- Faces detected will be saved in the dataset folder under your name.

### Option 2 (Recognize Faces):

- The model trains on all faces in the dataset folder.

- The webcam opens and tries to recognize faces live.

- Recognized faces are displayed with their names.

- Unknown faces are labeled “Unknown.”

- To stop recognition, interrupt the kernel (Ctrl+C).

