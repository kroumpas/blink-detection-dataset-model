# Blink Detection Dataset and Model

This repository contains the **dataset**, **trained neural network model**, and **scripts** used to identify and classify blinks as voluntary or involuntary based on eye openness signals. The methodology is grounded in recent research and improved using additional data preprocessing techniques.

---

## 🚀 Project Overview

Understanding and classifying blinks is essential for various applications such as human-computer interaction, fatigue monitoring, and medical diagnostics. This project builds upon the framework provided by [Nyström et al., 2024](https://doi.org/10.3758/s13428-023-02333-9), utilizing eye openness signals as a key indicator.

### Goals:
1. **Collect and preprocess** eye-tracking data to create a robust dataset.
2. **Train a neural network** to classify blinks as voluntary or involuntary.
3. Provide an open-access dataset and trained model to the research community.

---

## 📁 Repository Contents

- `dataset.csv`: Preprocessed dataset with blink duration and eye openness signals.
- `blink_classifier_model.h5`: Trained neural network model.
- `README.md`: Documentation for the repository.
- `LICENSE`: License details for usage and distribution.

---

## 📊 Dataset Description

The dataset includes eye openness data collected from **42 participants** across multiple conditions:
- **TOI (Time of Interest)**: Categorized as Blink Condition, Non-Blink Condition, and Entire Recording.
- **Features**:
  - `blink_duration`: Duration of the blink (in milliseconds).
  - `eye_openness_left`: Series of eye openness values for the left eye.
  - `eye_openness_right`: Series of eye openness values for the right eye.
- **Target**:
  - `blink_type`: Categorized as `Voluntary`, `Involuntary`, or `Invalid`.

---

## 🧠 Neural Network Model

The neural network is designed to classify blinks using blink duration and eye openness data:

### Architecture:
1. **Input Layer**: Features include `blink_duration`, `eye_openness_left`, and `eye_openness_right`.
2. **Hidden Layers**:
   - Two dense layers with ReLU activation.
   - Dropout layers to prevent overfitting.
3. **Output Layer**:
   - Softmax activation for classification.

### Performance:
- **Test Accuracy**: ~92% on the validation dataset.

---

## 📈 Results and Insights

The trained model effectively distinguishes between voluntary and involuntary blinks based on eye openness signals and blink duration. The use of eye openness as a feature provides a novel approach to blink detection, improving classification accuracy compared to traditional methods.

---

## 🛡️ License

This project is licensed under the [MIT License](LICENSE). You are free to use, modify, and distribute the dataset and code with attribution.

---

## 🤝 Contributing

Contributions are welcome! Please open an issue or submit a pull request to suggest improvements or report bugs.

---

## 📧 Contact

For questions or collaboration, feel free to contact:
- **Name**: Konstantinos Roumpas
- **Email**: k.roumpas@upatras.gr
