# CyberAttack Financial Loss Predictor

Developed a web-based prediction tool using neural networks and ridge regression to estimate the financial loss (in millions of USD) caused by cyberattacks. Built using Python, Streamlit, and machine learning libraries, this project was created during AI4ALL Ignite Accelerator as part of our exploration into applied AI and modeling.

---

## Problem Statement

Cyberattacks are growing in frequency, severity, and financial impact. However, most organizations lack a way to predict the potential loss of an attack before it happens. Our goal is to model historical global cyberattack data and provide a real-time tool for estimating financial damage based on factors such as attack type, industry, and vulnerability exploited.

---

## Key Results

- Cleaned and preprocessed global cybersecurity data (Kaggle 2015–2024).
- Built a neural network and ridge regression model to predict financial losses.
- Achieved a Mean Absolute Error (MAE) of 24.96 on test data.
- Integrated user input interface via Streamlit to allow scenario testing.

---

## Methodologies

To build an effective predictive model:

- We loaded and explored the dataset using `pandas`. We explored the correlation between variables. 
- One-hot encoded categorical variables such as country, industry, and attack type.
- Scaled numerical features using `StandardScaler` to prepare for model training.
- Used `SDV`'s `GaussianCopulaSynthesizer` to augment data with synthetic samples.
- Trained and evaluated two models:
  - **Ridge Regression**: Simpler, faster, and performed better on small datasets.
  - **Neural Network**: More complex and modern, allowing us to learn key deep learning concepts, even though it might not be as suitable as Ridge Regression.
---

## Why Two Models?

Although **ridge regression is more suitable than** neural network in this specific project due to the limited dataset size, we included the neural network for **educational purposes**:

We learned how to:

- Build multi-layer neural network architectures using TensorFlow/Keras.
- Apply regularization, dropout, and batch normalization to prevent overfitting.
- Use callbacks such as EarlyStopping and ReduceLROnPlateau for better training.
- Compare classical ML (ridge) vs deep learning models.
- Interpret MAE, RMSE, and residual plots.
- Deploy machine learning models via **Streamlit Cloud**.

Ultimately, **ridge regression** would be the better fit in real-world scenarios like this, due to its cost, speed, and interpretability on small-to-medium structured datasets.

---

## Live Demo

[Live Streamlit App](https://ai4allg16d-jznwalqkp7bva9k2dqg3ge.streamlit.app/)

---

## Data Source

- Kaggle: [Global Cybersecurity Threats 2015–2024](https://www.kaggle.com/)

---

## Technologies Used

- Python 3.10+
- pandas
- numpy
- scikit-learn
- TensorFlow / Keras
- SDV (Synthetic Data Vault)
- Streamlit
- Matplotlib / seaborn

---

## Setup Instructions

To run this project locally using Conda:

```bash
# 1. Clone the repository
$ git clone https://github.com/KhaiXin30/ai4allG16D.git

# 2. Create and activate a conda environment
$ conda create -n env_name python=3.10
$ conda activate env_name

# 3. Install dependencies
$ pip install -r requirements.txt

# 4. Run the Streamlit app
$ streamlit run streamlit_app.py
```

---

## Authors 

*This project was completed in collaboration with:*
- *Khai Xin ([kuankhaixin2003@gmail.com](mailto:jkuankhaixin2003@gmail.com))*
- *Stacy Albert ([stacyalbert9@gmail.com](stacyalbert9@gmail.com))*
- *Michael Amoako ([mamoako.1521@gmail.com](mailto:mamoako.1521@gmail.com))*
- *Aditya Senthil ([Adityasenthil0117@gmail.com](mailto:Adityasenthil0117@gmail.com))*



