# 🛒 Good Seed: Age Verification with Deep Learning

## 📌 Introduction
This project tackles a key challenge for the Good Seed supermarket chain: complying with alcohol sales regulations by preventing sales to underage customers. The goal is to build and evaluate a computer vision model that can estimate a person's age from a photograph, serving as a support tool for staff at the point of sale.

## 📂 Dataset
The model was trained on a dataset containing thousands of photographs of people with their corresponding real-world ages.

- **Root Directory:** `/datasets/faces/`
- **Images:** A folder (`final_files`) with 7,591 photos.
- **Labels:** A CSV file (`labels.csv`) with two columns: `file_name` and `real_age`.

## ⚙️ Methodology
The project was developed in four main phases:

### 1. Exploratory Data Analysis (EDA)
- Loaded the data and analyzed descriptive statistics for age.
- Visualized the age distribution to identify imbalances in the dataset.
- Reviewed a sample of images to understand the variety and quality of the data.

### 2. Model Development
- Utilized a Convolutional Neural Network (CNN) architecture based on **ResNet50**, leveraging transfer learning with pre-trained **ImageNet** weights.
- Modified the model's head for a regression task, with an output layer designed to predict a numerical value (age).

### 3. Model Training
- Trained the model on a GPU platform to accelerate the process.
- Used **Mean Absolute Error (MAE)** as the primary metric and loss function, with the **Adam** optimizer.
- Implemented data augmentation to improve the model's robustness and generalization.

### 4. Evaluation
- Evaluated the model's performance on the validation set, with the goal of achieving an MAE below 8.

## 📊 Key Analyses
- **Age Distribution:** The analysis revealed a higher concentration of data in the 20–40 age range.
- **Model Performance:** The final model achieved an MAE of **7.54**, meeting the project's requirements.
- **Practical Application:** Analyzed how the model can serve as an alert system for cashiers rather than an automated decision-making system.

## ✅ Conclusion
This project demonstrates the ability to develop an end-to-end computer vision solution, covering:

- Python (**Pandas**, **Matplotlib**, **Seaborn**)
- Deep Learning with **TensorFlow** and **Keras**
- Transfer Learning with **ResNet50**
- Image Processing and Data Augmentation
- Analysis of an AI model's feasibility for a real-world business problem

The developed model is a viable support tool that can help Good Seed reinforce its responsible sales policies.

## 💻 Tech Stack
- Python  
- Pandas  
- TensorFlow  
- Keras  
- Matplotlib  
- Seaborn  
- Jupyter Notebook  

## 🤝 Contact
Created by **[Your Name]**  
🔗 [LinkedIn](#) | [GitHub](#)
