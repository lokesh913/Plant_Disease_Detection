# Plant Disease Detection System

## Overview
This is a deep learning-based web application that can detect diseases in plants from their images. The system currently supports detection of three conditions in plants:
- Healthy
- Powdery Mildew
- Rust

## Features
- Web-based interface for easy interaction
- Real-time plant disease detection
- Support for image upload
- Built with Flask and TensorFlow
- Pre-trained deep learning model

## Tech Stack
- Python 3.x
- TensorFlow 2.x
- Flask
- OpenCV
- PIL (Python Imaging Library)
- HTML/CSS

## Project Structure
```
plant_disease_detection-main/
│
├── app.py                 # Main Flask application
├── model.h5              # Trained deep learning model
├── requirements.txt      # Project dependencies
├── Model_Training.ipynb  # Jupyter notebook for model training
│
├── static/              # Static files (CSS, JS, images)
├── templates/           # HTML templates
├── uploads/            # Folder for uploaded images
└── archive/           # Dataset and other resources
```

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/plant_disease_detection.git
cd plant_disease_detection
```

2. Create a virtual environment (recommended):
```bash
python -m venv .venv
```

3. Activate the virtual environment:
- On Windows:
```bash
.venv\Scripts\activate
```
- On macOS/Linux:
```bash
source .venv/bin/activate
```

4. Install the required dependencies:
```bash
pip install -r requirements.txt
```

## Usage

1. Make sure you're in the project directory and your virtual environment is activated.

2. Run the Flask application:
```bash
python app.py
```

3. Open your web browser and navigate to:
```
http://127.0.0.1:5000/
```

4. Upload an image of a plant leaf through the web interface.

5. The system will analyze the image and display whether the plant is:
   - Healthy
   - Affected by Powdery Mildew
   - Affected by Rust

## Model Information
- The model is trained using a deep learning architecture
- Training details can be found in `Model_Training.ipynb`
- The trained model is saved as `model.h5`
- The model achieves classification among three classes: Healthy, Powdery Mildew, and Rust

## Directory Structure Explained
- `app.py`: Contains the Flask application code and routing logic
- `model.h5`: The trained deep learning model
- `requirements.txt`: Lists all Python dependencies
- `Model_Training.ipynb`: Jupyter notebook containing the model training process
- `static/`: Contains static files like CSS, JavaScript, and images
- `templates/`: Contains HTML templates for the web interface
- `uploads/`: Temporary storage for uploaded images
- `archive/`: Contains the dataset and other resources

## Requirements
The main requirements are:
- tensorflow >= 2.0.0
- numpy >= 1.19.2
- Pillow >= 8.0.0
- opencv-python >= 4.5.0
- flask >= 2.0.0
- werkzeug >= 2.0.0

## Contributing
Feel free to fork this repository and submit pull requests. For major changes, please open an issue first to discuss what you would like to change.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Author
Lokesh Chavan

## Acknowledgments
- Dataset: [Plant Disease Recognition Dataset](https://www.kaggle.com/datasets/rashikrahmanpritom/plant-disease-recognition-dataset) by Rashik Rahman Pritom
