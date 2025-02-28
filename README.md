# AI-Generated Art Detection

This project focuses on distinguishing between **AI-generated art** and **human-created art** using advanced **Convolutional Neural Network (CNN)** architectures. The goal is to classify artworks into two categories: AI-generated or real (human-created). The project explores various deep learning models, including **VGGNet**, **ResNet**, and **DenseNet**, and evaluates their performance on different art styles and datasets.

---

## Features

- **Art Style Classification**: Classifies artworks into AI-generated or human-created categories.
- **Multiple Architectures**: Utilizes custom CNN architectures, VGGNet, ResNet, and DenseNet.
- **Data Preprocessing**: Includes image normalization and dataset preparation for training.
- **Two Training Phases**:
  - **First Phase**: Training on individual art styles (e.g., Realism, Renaissance, Surrealism).
  - **Second Phase**: Training on the entire dataset for generalization.
- **Evaluation**: Performance metrics such as accuracy, precision, recall, and F1-score are used to evaluate the models.

---

## Technologies Used

- **Python**: Primary programming language.
- **TensorFlow/Keras**: For building and training deep learning models.
- **Pandas/NumPy**: For data manipulation and preprocessing.
- **Matplotlib/Seaborn**: For data visualization.
- **Scikit-learn**: For evaluation metrics.
- **Git**: For version control.

---

## Installation

### Prerequisites
- Python 3.8 or higher
- pip (Python package installer)

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/Aziz16KH/ai-art-detection.git
   cd ai-art-detection
   ```
2. Create a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

---

## Usage

### Data Preprocessing
1. Place your dataset in the `data/` directory.
2. Run the preprocessing script:
   ```bash
   python scripts/preprocess_data.py
   ```

### Model Training
1. Train the model using the preprocessed data:
   ```bash
   python scripts/train_model.py
   ```
2. The trained model will be saved in the `models/` directory.

### Evaluation
1. Evaluate the model's performance:
   ```bash
   python scripts/evaluate_model.py
   ```

---

## Results

### First Training Phase (Individual Art Styles)
- The model was trained on individual art styles, including **Realism**, **Renaissance**, **Surrealism**, and others.
- Performance metrics (accuracy, precision, recall, F1-score) were recorded for each style.

### Second Training Phase (Entire Dataset)
- The model was trained on the entire dataset using advanced architectures like **VGGNet**, **ResNet**, and **DenseNet**.
- The **Second CNN** architecture achieved the best performance with **94% accuracy**.

### Testing on a Second Dataset
- The models were tested on a separate dataset for generalization.
- Results showed that the models performed well on human-created art but struggled with AI-generated art (50% accuracy).

---

## Key Findings

- **Best Model**: The custom **Second CNN** architecture achieved the highest accuracy (94%) on the entire dataset.
- **ResNet Performance**: ResNet also performed well, benefiting from residual connections that mitigate vanishing gradients.
- **DenseNet Performance**: DenseNet performed slightly worse (92%) but still demonstrated strong classification capabilities.
- **Generalization**: Models trained on the entire dataset generalized better than those trained on individual art styles.

---

## Contributing

Contributions are welcome! If you'd like to improve this project, follow these steps:
1. Fork the repository.
2. Create a new branch: `git checkout -b feature/your-feature-name`.
3. Commit your changes: `git commit -m "Add your message here"`.
4. Push to the branch: `git push origin feature/your-feature-name`.
5. Open a pull request and describe your changes.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Acknowledgments

- **Supervisor**: Prof. Carmen BISOGNI
- **Candidates**: Mohamed Aziz KHITMI, Zakarya BOUDRAF, Melissa OULD BRAHAM
- **Università degli Studi di Salerno**: For providing the resources and support for this project.

---

## Contact

For questions or feedback, feel free to reach out:

- **Author**: Mohamed Aziz KHITMI
- **GitHub**: [Aziz16KH](https://github.com/Aziz16KH)
