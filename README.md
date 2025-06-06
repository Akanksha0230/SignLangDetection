# **Sign Language Detection**


This project implements a real-time **Sign Language Detection** system using computer vision and machine learning. It captures hand gestures from webcam input, trains a model, and predicts sign language characters live.

### **Features:**
- Real-time sign detection using webcam input.
- Custom dataset collection through key-triggered captures.
- Trains a machine learning model on image data.
- Predicts hand signs and displays corresponding characters.

### **Prerequisites:**

Before you begin, ensure you have the following installed:

- Anaconda or Miniconda
- Python 3.9.13

## **Setup Instructions**

1. Create the virtual environment
```
    python -m venv sign
    ```
2. Activate the Environment:
   - Activate the newly created environment with:
```
sign\Scripts\activate  # On Windows
```
3. Install Requirements:
   - Install the necessary dependencies using pip:
     ```
     pip install -r requirements.txt
     ```
4. Run the Application:

Step 1: Collect Sign Language Data
``` python collectdata.py ```

*A webcam window will open. In the blue frame, show your hand sign. Press the corresponding character key (e.g., A, B, etc.) on your keyboard. Each keypress captures an image. The more keypresses, the more samples you collect for that sign.

Step 2: Convert Data to NumPy Format
``` python data.py```
This script processes and saves the collected image data into NumPy arrays for training.

Step 3: Train the Model
``` python trainmodel.py```
This trains a machine learning model using the saved image arrays.

Step 4: Run the Sign Detection App
``` python app.py ```
A webcam window will appear. Show a hand sign inside the frame. The trained model will predict the corresponding character in real time.

### **Usage:**

Activate the virtual environment and run the scripts in sequence to collect sign images, convert them to NumPy arrays, and train the model. Use your webcam to display hand signs, and press corresponding keys to label them during data collection. Once trained, run app.py to start real-time detection. The system will predict and display the corresponding character for the hand sign shown in the camera frame.