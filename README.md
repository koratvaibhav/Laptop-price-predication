# 💻 Laptop Price Prediction using Machine Learning

## 📌 Project Overview
This project aims to predict the price of laptops based on their technical specifications using various machine learning models, with a focus on **Support Vector Regression (SVR)**. The dataset includes attributes like brand, processor type, RAM, storage, display size, operating system, and more. The model helps understand how these specifications influence laptop pricing.

---

## 📊 Dataset Description

Each row in the dataset represents a laptop with the following features:

| Column Name              | Description                              |
|--------------------------|------------------------------------------|
| `Name`                   | Laptop model name                        |
| `Brand`                  | Manufacturer (e.g., HP, Dell, Lenovo)   |
| `Price`                  | Laptop price (Target Variable)          |
| `Rating`                 | Customer rating                         |
| `Processor_brand`        | Brand of processor (Intel/AMD)          |
| `Processor_gen`          | Processor generation                    |
| `Core_per_processor`     | Number of cores                         |
| `Energy_Efficient_Units` | Power efficiency flag                   |
| `RAM_GB`                 | RAM size in GB                          |
| `RAM_type`               | Type of RAM (e.g., DDR4)                |
| `Storage_capacity_GB`    | Total storage in GB                     |
| `Storage_type`           | Type of storage (HDD, SSD)              |
| `Graphics_brand`         | GPU brand                               |
| `Display_size_inches`    | Screen size                             |
| `Horizontal_pixel`       | Screen resolution (width)               |
| `Vertical_pixel`         | Screen resolution (height)              |
| `Touch_screen`           | Whether the screen is touch-enabled     |
| `Operating_system`       | OS (e.g., Windows, macOS)               |

---

## 🧠 Machine Learning Approach

### 🔍 Problem Type
- **Supervised Learning**
- **Regression Task** (predicting continuous `Price`)

### 📌 Models Implemented
- ✅ **Support Vector Regression (SVR)**
- ✅ Random Forest Regressor *(for comparison)*
- ✅ Linear Regression *(baseline)*

### 🔧 Preprocessing Steps
- Handled missing values using forward-fill
- Outlier detection and removal using the IQR method
- Categorical encoding with One-Hot Encoding
- Feature scaling with StandardScaler (for SVR)
- Train-Test split (80-20)

---

## 🧪 Evaluation Metrics
- **R² Score**
- **Mean Absolute Error (MAE)**
- **Mean Squared Error (MSE)**

---

## 📈 Results

| Model                  | R² Score | MAE (Approx) |
|------------------------|----------|--------------|
| Support Vector Regressor (SVR) | 0.78     | ~3200 ₹     |
| Random Forest Regressor       | 0.89     | ~2100 ₹     |
| Linear Regression             | 0.70     | ~4000 ₹     |

*(Values are for illustrative purposes. Actual results may vary based on the dataset



