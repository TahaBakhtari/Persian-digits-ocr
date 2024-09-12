
# Persian-Digits-OCR
### (Handwrite) 
neural network "DeepLearning"

This project focuses on recognizing Persian digits using a deep learning-based Optical Character Recognition (OCR) system. The model has been trained on a custom dataset of Persian digits, and the pre-trained model is available for immediate use.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Dataset](#dataset)
- [Pre-Trained Model](#pre-trained-model)
- [License](#license)

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/tahabakhtari/Persian-digits-ocr.git
   ```
2. **Install required dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

Run the Jupyter notebook to perform Persian digit recognition:

1. Load the Persian digit dataset.
2. Preprocess the dataset to fit the model's input requirements.
3. Use the pre-trained model for predictions or train a new model.
4. Evaluate the model's performance on test data.

```bash
jupyter notebook code.ipynb
```

### Using the Pre-Trained Model

To use the pre-trained model, load the model file and run predictions directly on your input images:

```python
from keras.models import load_model

model = load_model('models/persian_digit_model.h5')
# Use the model for predictions
predictions = model.predict(input_data)
```

## Project Structure

- **`code.ipynb`**: The core notebook that includes data loading, model training, and prediction steps.
- **`data/`**: Directory containing the dataset of Persian digit images.
- **`models/`**: Contains the pre-trained model (`persian_digit_model.h5`).
- **`utils.py`**: Helper functions for data preprocessing and evaluation.

## Dataset

The dataset consists of Persian digit images (0-9) that have been preprocessed and formatted for model training. These images are available in the `data/` folder, and can be directly used to retrain or fine-tune the model.

## Pre-Trained Model

A pre-trained model is included in the `models/` directory. You can load and use this model without needing to retrain. The model has been trained on thousands of Persian digit samples to ensure accurate recognition.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
