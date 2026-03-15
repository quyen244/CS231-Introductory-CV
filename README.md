<p align="center"> 
  <a href="https://www.uit.edu.vn/" title="University of Information Technology" style="border: none;">
    <img src="https://i.imgur.com/WmMnSRt.png" alt="University of Information Technology (UIT)">
  </a>
</p>

<h1 align="center"><b>CS231 - Introduction to Computer Vision</b></h1>

# **Course Repository: CS231 - Introduction to Computer Vision**

> **CS231 – Introduction to Computer Vision** là repository cá nhân dùng để lưu trữ code, notebook và tài liệu trong quá trình học môn **Nhập môn Thị giác Máy tính**. Repository này bao gồm các bài thực hành (labs) tập trung vào việc xử lý ảnh, trích xuất đặc trưng màu sắc và áp dụng các thuật toán Machine Learning cơ bản để giải quyết bài toán phân loại hình ảnh.

<p align="center">
  <img src="thumbnail.png" width="600" alt="thumbnail">
</p>

---

# 📚 Course Overview

Khóa học giới thiệu các kiến thức nền tảng của **Computer Vision**, bao gồm:

- Image representation
- Color spaces
- Feature extraction
- Image classification
- Traditional machine learning for vision tasks

Các bài thực hành được tổ chức theo **từng lab** để thực nghiệm các phương pháp khác nhau.

---

# 🧪 Labs

## 🔬 Lab 1 — Color Feature Extraction & KNN Classification

Lab 1 tập trung vào việc **trích xuất đặc trưng màu sắc từ ảnh** và sử dụng các thuật toán Machine Learning cơ bản để thực hiện phân loại hình ảnh.

### Nội dung chính

- Đọc và xử lý ảnh bằng **OpenCV**
- Tiền xử lý dataset ảnh
- Trích xuất đặc trưng màu sắc

### Các đặc trưng được sử dụng

1. **RGB Histogram**
   - 256 bins cho mỗi kênh màu
   - Tạo vector đặc trưng 768 chiều

2. **HSV Histogram**
   - Histogram 3 chiều
   - Sử dụng cấu hình **8×8×8 bins**

3. **Color Moments**
   - Mean
   - Standard deviation
   - Skewness

4. **Dominant Color**
   - Sử dụng thuật toán **K-Means clustering** để tìm màu chủ đạo

### Pipeline

```

Image
↓
Feature Extraction
↓
Feature Vector
↓
Train KNN Classifier
↓
Evaluate Accuracy

```

### Thực nghiệm

So sánh độ chính xác giữa các loại đặc trưng:

- HSV Histogram
- Color Moments
- Dominant Color

---

## 🔬 Lab 2 — Logistic Regression & SGDClassifier

Lab 2 tập trung vào việc **thực nghiệm các thuật toán phân loại tuyến tính** cho bài toán Computer Vision.

### Thuật toán được sử dụng

- Logistic Regression
- SGDClassifier (Stochastic Gradient Descent)

### Nội dung chính

- Huấn luyện mô hình phân loại ảnh
- So sánh hiệu năng giữa các mô hình
- Tối ưu tham số bằng **Grid Search**

### Pipeline

```

Feature Vector
↓
Model Training
↓
Hyperparameter Tuning (GridSearchCV)
↓
Evaluation

```

### Mục tiêu thực nghiệm

- So sánh độ chính xác giữa:
  - Logistic Regression
  - SGDClassifier
- Tìm bộ tham số tối ưu bằng **GridSearchCV**

---

# 🛠 Technologies Used

Các thư viện chính được sử dụng trong repository:

- Python
- NumPy
- OpenCV
- Pillow (PIL)
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

# 📂 Repository Structure

```

CS231-Computer-Vision/
│
├── datasets/                # Image datasets
├── notebooks/               # Jupyter notebooks for experiments
│
├── lab1_color_features.ipynb
├── lab2_linear_models.ipynb
│
├── src/
│   ├── feature_extraction
│   └── models
│
├── README.md
└── requirements.txt

```

---

# 🎯 Learning Outcomes

Sau khi hoàn thành các lab trong repository này, bạn có thể:

- Hiểu cách biểu diễn ảnh trong máy tính
- Trích xuất đặc trưng màu sắc từ ảnh
- Xây dựng pipeline cho bài toán **image classification**
- Áp dụng các thuật toán Machine Learning cơ bản cho Computer Vision

---

# 👤 Author

**Quyen**

Student - University of Information Technology (UIT)


