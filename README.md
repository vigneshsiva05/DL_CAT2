# DL_CAT2

# 🌧️ Rainfall Prediction Using LSTM

## 📌 About the Project

Rainfall prediction plays an important role in agriculture, water resource management, and flood prevention. In this project, I developed a rainfall prediction model using **Long Short-Term Memory (LSTM)**, a deep learning algorithm designed to learn patterns from sequential data.

I used the IMD Rainfall Dataset 2022 from Kaggle and Google Colab to train the model and predict daily rainfall for Coimbatore, Tamil Nadu.

This project helped me understand how deep learning can be applied to real-world weather prediction problems.

## 🎯 Objectives

- Predict daily rainfall using historical rainfall data.
- Learn how LSTM works with time-series data.
- Preprocess and normalize rainfall data.
- Evaluate the model using different performance metrics.
- Visualize actual and predicted rainfall.

## 📂 Dataset

**Dataset:** IMD Rainfall Dataset 2022

**Source:** [Kaggle – IMD Rainfall Dataset 2022](https://www.kaggle.com/datasets/ankitgaikar1995/imd-rainfall-dataset-2022)

The dataset contains state, district, month, and daily rainfall measurements. For this project, I selected rainfall data for Coimbatore, Tamil Nadu.

## 🛠️ Technologies Used

- Python
- Google Colab
- Pandas and NumPy
- Matplotlib
- Scikit-learn
- TensorFlow and Keras
- LSTM Deep Learning Model

## ⚙️ Project Workflow

### 1. Dataset Loading
I loaded the rainfall dataset into Google Colab using Pandas and selected the required district.

### 2. Data Preprocessing
I converted monthly records into daily rainfall data, handled missing values, removed invalid negative values, and applied logarithmic transformation and MinMax scaling.

### 3. Dataset Splitting
I divided the dataset chronologically into 80% training data and 20% testing data.

### 4. Model Training
I built an LSTM model using TensorFlow and Keras. The previous 14 days of rainfall were used to predict the next day's rainfall. I also used Dropout and Early Stopping to help reduce overfitting.

### 5. Prediction and Evaluation
I evaluated the model by comparing predicted rainfall with actual rainfall using tolerance-based accuracy, Mean Absolute Error (MAE), and Root Mean Squared Error (RMSE).

### 6. Visualization
I plotted graphs to compare actual and predicted rainfall and understand the model's performance.

## 📊 Model Performance

The model produced the following results on the test dataset:

| Metric | Result |
|---|---:|
| Accuracy within ±5 mm | 83.56% |
| Mean Absolute Error (MAE) | 2.883 mm |
| Root Mean Squared Error (RMSE) | 5.971 mm |

**Note:** The 83.56% value represents a custom tolerance-based metric: the percentage of test predictions within ±5 mm of actual rainfall. It is not standard classification accuracy.

## 🚀 How to Run the Project

1. Download or clone this repository.
2. Open Google Colab at https://colab.research.google.com/.
3. Upload or open the project notebook.
4. Download the dataset from the Kaggle link above.
5. Upload the dataset when prompted by the notebook.
6. Run each code cell in order.
7. Review the prediction results and graphs.

## 🌱 Applications

- Agricultural planning and irrigation
- Water resource management
- Flood risk assessment
- Rainfall monitoring
- Weather data analysis

## ⚠️ Limitations

This project uses rainfall data from a single year, so it may not capture long-term seasonal patterns. Rainfall prediction can also be affected by temperature, humidity, wind, and other weather conditions. The results should therefore be treated as experimental rather than as an operational weather forecast.

## 📚 What I Learned

Through this project, I learned how to preprocess time-series data, build and train an LSTM model, evaluate regression predictions, and visualize model results using Python. It also helped me understand how deep learning can be applied to real-world problems.

## 👨‍💻 Author

Developed as a learning project to explore deep learning and rainfall prediction using Python.

## ⭐ Conclusion

This project demonstrates how an LSTM model can learn patterns from historical rainfall data to predict daily rainfall. It was a useful hands-on experience in deep learning, time-series analysis, and model evaluation.
