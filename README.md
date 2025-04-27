# 📝 Project Title:
Handwritten Digit Recognition 

# 📚 Project Description:
This project builds a system that:
1. Trains a CNN model to recognize handwritten digits (0-9) using the MNIST dataset.
2. Tests and evaluates the model’s performance.
3. Deploys the model using a simple GUI with Tkinter where users can draw digits and get predictions.

Handwritten-Digit-Recognition: 
The Handwritten Digit Recognition project aims to build an intelligent system that can automatically recognize digits (0–9) written by hand.The project also includes a Graphical User Interface (GUI), allowing users to draw digits and instantly receive predictions.

# 🏗️ Project Steps:
1. Import Libraries
TensorFlow, Keras, NumPy, Matplotlib, Tkinter, PIL, etc.

2. Load and Preprocess Data
 * Load the MNIST dataset.
 * Normalize images (pixel values 0-255 → 0-1).
 * Reshape images to (28, 28, 1) for CNN input.

3. Build the CNN Model
Layers:
* Conv2D → MaxPooling2D → Conv2D → MaxPooling2D → Conv2D
* Flatten
* Dense(64)
* Dense(10) with softmax activation (for multi-class classification)

4. Compile the Model
  * Optimizer: Adam
  * Loss: Sparse Categorical Crossentropy
  * Metric: Accuracy

5. Train the Model
  * Trained for 20 epochs with validation on test data.

6. Evaluate the Model
   * Test accuracy is printed.
   * Predictions are plotted for individual samples and multiple samples.

7. Save the Model
   * Model saved as: mnist_digit_recognition_model.h5

8. GUI Application
   * Built using Tkinter.
   * You can draw a digit on a white canvas.
 Two buttons:
  - Predict (to show the model’s prediction)
  - Clear (to reset the canvas)

✨ Features:
- Interactive notebook with visualization.
- Interactive slider to browse predictions on test images.
- Deployable GUI using Tkinter.

⚡ Quick Summary:
* ✅ Data: MNIST handwritten digits
* ✅ Model: CNN with 3 Convolutions + Dense layers
* ✅ Deployment: Tkinter GUI + Canvas drawing

- Disadvantage:
  * Only we can Predict from 0-9.
  * It can predict Only Single digits.
     
-----Note-----
Install the required libraries and run the project in juypter notebook. to install the required libraries just refer the requirement file and create a virtual env in project folder and start installing using : 
* pip intall   # using cmd 
* !pip install  # using jupyter notebook


# Output:
* empty canvas
  <img width="942" alt="image" src="https://github.com/user-attachments/assets/3e9ae0dd-71f2-4568-a55e-ad28b8a0a92b" />




* Hand written number on canva and predicted output
  
  <img width="151" alt="image" src="https://github.com/user-attachments/assets/0e9f7003-ac0e-45c3-9881-20fe4eed4c82" />      <img width="150" alt="image" src="https://github.com/user-attachments/assets/b5568359-0283-4d90-88a7-9e596d4608aa" />      <img width="150" alt="image" src="https://github.com/user-attachments/assets/4084a238-c70a-4cdb-99dd-4fbfe2b78c02" />


